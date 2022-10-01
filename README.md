  plr = game.Players.LocalPlayer
    mouse = plr:GetMouse()
    mouse.KeyDown:connect(function(key)
        if key == "z" then
		local Plr = game.Players.LocalPlayer



local Tool = '[Boombox]' 

local plr = game.Players.LocalPlayer
local char = plr.Character
local bp = plr.Backpack



        if char:FindFirstChild(Tool) then
            char:FindFirstChild(Tool).Parent = bp
        else
            bp:FindFirstChild(Tool).Parent = char
        end
    
        local args = {
    [1] = "Boombox",
    [2] = "6721974349"
}

game:GetService("ReplicatedStorage").MainEvent:FireServer(unpack(args))

    
 wait(3)
    
local args = {
    [1] = "BoomboxStop"
}

game:GetService("ReplicatedStorage").MainEvent:FireServer(unpack(args))


wait(0.2)

Plr.Character.Humanoid:UnequipTools()



end
end) 
