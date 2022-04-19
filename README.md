while wait(1.2) do

for i,v in pairs(game:GetService("Workspace").Items:GetDescendants()) do

if v.Name == "TouchInterest"  then

local CFrameEnd  = v.Parent.CFrame --ใส่CFrame
local Time = 1 --ใส่เวลาที่จะไปถึง
local tween = game:GetService("TweenService"):Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(Time), {CFrame = CFrameEnd}) tween:Play()

end
end
end
