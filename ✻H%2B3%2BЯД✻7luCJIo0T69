local HackingLife = Instance.new("ScreenGui")
local HL = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")
local TextLabel_2 = Instance.new("TextLabel")
local TextButton = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local TextButton_2 = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local Credits = Instance.new("TextLabel")
local UICorner_4 = Instance.new("UICorner")
local TextButton_3 = Instance.new("TextButton")
local UICorner_5 = Instance.new("UICorner")
local GAW = Instance.new("TextButton")
local UICorner_6 = Instance.new("UICorner")
local TextButton_4 = Instance.new("TextButton")
local UICorner_7 = Instance.new("UICorner")
local TextButton_5 = Instance.new("TextButton")
local UICorner_8 = Instance.new("UICorner")
local TextButton_6 = Instance.new("TextButton")
local UICorner_9 = Instance.new("UICorner")
local TextButton_7 = Instance.new("TextButton")
local UICorner_10 = Instance.new("UICorner")

-- Properties

HackingLife.Name = "Hacking Life"
HackingLife.Parent = game.CoreGui
HackingLife.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
game.StarterGui:SetCore("SendNotification", {Title="Thanks"; Text="Thanks For Using Hacking Life!"; Duration=3;})

HL.Name = "HL"
HL.Parent = HackingLife
HL.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
HL.BorderColor3 = Color3.new(0, 0, 0)
HL.BorderSizePixel = 0
HL.Position = UDim2.new(0.463281035, 0, 0.25746268, 0)
HL.Size = UDim2.new(0, 140, 0, 389)
HL.Active = true
HL.Draggable = true

UICorner.Parent = HL

TextLabel.Parent = HL
TextLabel.BackgroundColor3 = Color3.new(1, 1, 1)
TextLabel.BackgroundTransparency = 1
TextLabel.BorderColor3 = Color3.new(0, 0, 0)
TextLabel.BorderSizePixel = 0
TextLabel.Position = UDim2.new(-0.635023713, 0, -0.0245259907, 0)
TextLabel.Size = UDim2.new(0, 319, 0, 50)
TextLabel.Font = Enum.Font.Jura
TextLabel.Text = "Hacking Life"
TextLabel.TextColor3 = Color3.new(1, 1, 1)
TextLabel.TextSize = 24

TextLabel_2.Parent = HL
TextLabel_2.BackgroundColor3 = Color3.new(1, 1, 1)
TextLabel_2.BorderColor3 = Color3.new(0, 0, 0)
TextLabel_2.BorderSizePixel = 0
TextLabel_2.Position = UDim2.new(0, 0, 0.0978981629, 0)
TextLabel_2.Size = UDim2.new(0, 140, 0, 1)
TextLabel_2.Font = Enum.Font.SourceSans
TextLabel_2.Text = ""
TextLabel_2.TextColor3 = Color3.new(0, 0, 0)
TextLabel_2.TextSize = 14

TextButton.Parent = HL
TextButton.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton.BorderColor3 = Color3.new(0, 0, 0)
TextButton.BorderSizePixel = 0
TextButton.Position = UDim2.new(0.0804521814, 0, 0.124017082, 0)
TextButton.Size = UDim2.new(0, 118, 0, 28)
TextButton.Font = Enum.Font.Jura
TextButton.Text = "ESP"
TextButton.TextColor3 = Color3.new(1, 1, 1)
TextButton.TextSize = 19
TextButton.TextWrapped = true
TextButton.MouseButton1Down:Connect(function()
    local Players = game:GetService("Players")
    local RunService = game:GetService("RunService")
    local highlight = Instance.new("Highlight")
    highlight.Name = "Highlight"
    highlight.FillTransparency = 1 -- Make the fill fully transparent
    highlight.OutlineColor = Color3.new(0, 1, 0) -- Green outline color

    while true do
        wait(1) -- Wait for 1 second before refreshing

        for _, player in pairs(Players:GetChildren()) do
            local hrp = player.Character and player.Character:FindFirstChild("HumanoidRootPart")
            if hrp then
                local existingHighlight = hrp:FindFirstChild("Highlight")
                if existingHighlight then
                    existingHighlight:Destroy()
                end

                -- Clone and configure the highlight
                local highlightClone = highlight:Clone()
                highlightClone.Adornee = player.Character
                highlightClone.Parent = hrp
                highlightClone.DepthMode = Enum.HighlightDepthMode.AlwaysOnTop

                -- Create a BillboardGui to display the player's username and health
                local billboard = Instance.new("BillboardGui")
                billboard.Size = UDim2.new(0, 200, 0, 100) -- Increased height to fit both labels
                billboard.StudsOffset = Vector3.new(0, 3, 0) -- Position above the HRP
                billboard.AlwaysOnTop = true
                billboard.Adornee = hrp

                -- Username label
                local nameLabel = Instance.new("TextLabel")
                nameLabel.Size = UDim2.new(1, 0, 0.5, 0) -- Half height for the username
                nameLabel.Text = player.Name
                nameLabel.BackgroundTransparency = 1
                nameLabel.TextColor3 = Color3.new(1, 1, 1) -- White text color
                nameLabel.TextScaled = false
                nameLabel.TextSize = 14 -- Smaller text size
                nameLabel.Parent = billboard

                -- Health label
                local healthLabel = Instance.new("TextLabel")
                healthLabel.Size = UDim2.new(1, 0, 0.5, 0) -- Half height for the health display
                healthLabel.Position = UDim2.new(0, 0, 0.5, 0) -- Position it below the username
                healthLabel.BackgroundTransparency = 1
                healthLabel.TextColor3 = Color3.new(1, 1, 1) -- White text color for health
                healthLabel.TextScaled = false
                healthLabel.TextSize = 14 -- Smaller text size
                healthLabel.Parent = billboard

                -- Update health in real-time
                local humanoid = player.Character:FindFirstChild("Humanoid")
                if humanoid then
                    local function updateHealth()
                        healthLabel.Text = "Health: " .. math.floor(humanoid.Health)
                    end

                    humanoid:GetPropertyChangedSignal("Health"):Connect(updateHealth)
                    updateHealth()
                end

                billboard.Parent = hrp
            end
        end
    end
end)

UICorner_2.Parent = TextButton

TextButton_2.Parent = HL
TextButton_2.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton_2.BorderColor3 = Color3.new(0, 0, 0)
TextButton_2.BorderSizePixel = 0
TextButton_2.Position = UDim2.new(0.0804521814, 0, 0.220435679, 0)
TextButton_2.Size = UDim2.new(0, 118, 0, 28)
TextButton_2.Font = Enum.Font.Jura
TextButton_2.Text = "Kill Aura"
TextButton_2.TextColor3 = Color3.new(1, 1, 1)
TextButton_2.TextSize = 19
TextButton_2.TextWrapped = true
TextButton_2.MouseButton1Down:Connect(function()
	while wait () do
		for i, e in pairs(game.Players:GetChildren()) do
			if e ~= game.Players.LocalPlayer then
				local meleeEvent = game:GetService("ReplicatedStorage").meleeEvent
				meleeEvent:FireServer(e)

			end end end 
end)

UICorner_3.Parent = TextButton_2

Credits.Name = "Credits"
Credits.Parent = HL
Credits.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
Credits.BorderColor3 = Color3.new(0, 0, 0)
Credits.BorderSizePixel = 0
Credits.Position = UDim2.new(0.0783556253, 0, 0.905013263, 0)
Credits.Size = UDim2.new(0, 118, 0, 28)
Credits.Font = Enum.Font.Jura
Credits.Text = "By _.75f"
Credits.TextColor3 = Color3.new(1, 1, 1)
Credits.TextSize = 19

UICorner_4.Parent = Credits

TextButton_3.Parent = HL
TextButton_3.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton_3.BorderColor3 = Color3.new(0, 0, 0)
TextButton_3.BorderSizePixel = 0
TextButton_3.Position = UDim2.new(0.079864502, 0, 0.314250559, 0)
TextButton_3.Size = UDim2.new(0, 118, 0, 28)
TextButton_3.Font = Enum.Font.Jura
TextButton_3.Text = "Remove Doors"
TextButton_3.TextColor3 = Color3.new(1, 1, 1)
TextButton_3.TextSize = 14
TextButton_3.TextWrapped = true
TextButton_3.MouseButton1Down:connect(function()
	game.Workspace.Prison_Cellblock.doors:Destroy()

	for i,v in pairs(workspace:GetChildren())do
		if v.Name == "Doors" then
			v:Destroy()
		end
	end
end)

UICorner_5.Parent = TextButton_3

GAW.Name = "GAW"
GAW.Parent = HL
GAW.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
GAW.BorderColor3 = Color3.new(0, 0, 0)
GAW.BorderSizePixel = 0
GAW.Position = UDim2.new(0.0793448314, 0, 0.403742552, 0)
GAW.Size = UDim2.new(0, 118, 0, 28)
GAW.Font = Enum.Font.Jura
GAW.Text = "Fly [E]"
GAW.TextColor3 = Color3.new(1, 1, 1)
GAW.TextSize = 14
GAW.TextWrapped = true
GAW.MouseButton1Down:Connect(function()

	--Waits until the player is in game
	repeat wait()
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("Torso") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid")
	local mouse = game.Players.LocalPlayer:GetMouse()

	--Waits until the player's mouse is found
	repeat wait() until mouse

	--Variables
	local plr = game.Players.LocalPlayer
	local torso = plr.Character.Torso
	local flying = true
	local deb = true
	local ctrl = {f = 0, b = 0, l = 0, r = 0}
	local lastctrl = {f = 0, b = 0, l = 0, r = 0}
	local maxspeed = 50
	local speed = 0
	local bg = nil
	local bv = nil

	--Actual flying
	function Fly()
		bg = Instance.new("BodyGyro", torso)
		bg.P = 9e4
		bg.maxTorque = Vector3.new(9e9, 9e9, 9e9)
		bg.cframe = torso.CFrame
		bv = Instance.new("BodyVelocity", torso)
		bv.velocity = Vector3.new(0,0.1,0)
		bv.maxForce = Vector3.new(9e9, 9e9, 9e9)
		repeat wait()
			plr.Character.Humanoid.PlatformStand = true
			if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then
				speed = speed+.5+(speed/maxspeed)
				if speed > maxspeed then
					speed = maxspeed
				end
			elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then
				speed = speed-1
				if speed < 0 then
					speed = 0
				end
			end
			if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then
				bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
				lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r}
			elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then
				bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
			else
				bv.velocity = Vector3.new(0,0.1,0)
			end
			bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0)
		until not flying
		ctrl = {f = 0, b = 0, l = 0, r = 0}
		lastctrl = {f = 0, b = 0, l = 0, r = 0}
		speed = 0
		bg:Destroy()
		bg = nil
		bv:Destroy()
		bv = nil
		plr.Character.Humanoid.PlatformStand = false
	end

	--Controls
	mouse.KeyDown:connect(function(key)
		if key:lower() == "e" then
			if flying then 
				flying = false
			else
				flying = true
				Fly()
			end
		elseif key:lower() == "w" then
			ctrl.f = 1
		elseif key:lower() == "s" then
			ctrl.b = -1
		elseif key:lower() == "a" then
			ctrl.l = -1
		elseif key:lower() == "d" then
			ctrl.r = 1
		end
	end)

	mouse.KeyUp:connect(function(key)
		if key:lower() == "w" then
			ctrl.f = 0
		elseif key:lower() == "s" then
			ctrl.b = 0
		elseif key:lower() == "a" then
			ctrl.l = 0
		elseif key:lower() == "d" then
			ctrl.r = 0
		end
	end)

	Fly()
end)

UICorner_6.Parent = GAW

TextButton_4.Parent = HL
TextButton_4.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton_4.BorderColor3 = Color3.new(0, 0, 0)
TextButton_4.BorderSizePixel = 0
TextButton_4.Position = UDim2.new(0.079864502, 0, 0.496189147, 0)
TextButton_4.Size = UDim2.new(0, 118, 0, 28)
TextButton_4.Font = Enum.Font.Jura
TextButton_4.Text = "Enter Prison"
TextButton_4.TextColor3 = Color3.new(1, 1, 1)
TextButton_4.TextSize = 19
TextButton_4.TextWrapped = true
TextButton_4.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(918.77,100,2379.07)
	wait()
end)

UICorner_7.Parent = TextButton_4

TextButton_5.Parent = HL
TextButton_5.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton_5.BorderColor3 = Color3.new(0, 0, 0)
TextButton_5.BorderSizePixel = 0
TextButton_5.Position = UDim2.new(0.0800027028, 0, 0.592357934, 0)
TextButton_5.Size = UDim2.new(0, 118, 0, 28)
TextButton_5.Font = Enum.Font.Jura
TextButton_5.Text = "Escape Prison"
TextButton_5.TextColor3 = Color3.new(1, 1, 1)
TextButton_5.TextSize = 19
TextButton_5.TextWrapped = true
TextButton_5.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-905.213562, 91.627182, 2133.9707, 0, 0, -1, 0, 1, 0, 1, 0, 0)
	wait()
end)

UICorner_8.Parent = TextButton_5

TextButton_6.Parent = HL
TextButton_6.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton_6.BorderColor3 = Color3.new(0, 0, 0)
TextButton_6.BorderSizePixel = 0
TextButton_6.Position = UDim2.new(0.0800027028, 0, 0.692386866, 0)
TextButton_6.Size = UDim2.new(0, 118, 0, 28)
TextButton_6.Font = Enum.Font.Jura
TextButton_6.Text = "Mod Gun"
TextButton_6.TextColor3 = Color3.new(1, 1, 1)
TextButton_6.TextSize = 19
TextButton_6.TextWrapped = true
TextButton_6.MouseButton1Down:Connect(function()
	local gun1 = require(game.Players.LocalPlayer.Backpack["Remington 870"].GunStates)
	local gun2 = require(game.Players.LocalPlayer.Backpack["AK-47"].GunStates)
	local gun3 = require(game.Players.LocalPlayer.Backpack["M9"].GunStates)
	for i,v in pairs(gun1) do print(i,v) end
	for i,b in pairs(gun2) do print(i,b) end
	for i,a in pairs(gun3) do print(i,a) end
	gun1["AutoFire"] = true
	gun2["AutoFire"] = true
	gun3["AutoFire"] = true
	gun1["FireRate"] = 0.0001
	gun1["Spread"] = 0
	gun1["CurrentAmmo"] = 99999999999
	gun1["StoredAmmo"] = 99999999999
	gun2["FireRate"] = 0.0001
	gun2["Spread"] = 0
	gun2["CurrentAmmo"] = 99999999999
	gun2["StoredAmmo"] = 99999999999
	gun3["FireRate"] = 0.0001
	gun3["Spread"] = 0
	gun3["CurrentAmmo"] = 99999999999
	gun3["StoredAmmo"] = 99999999999
end)

UICorner_9.Parent = TextButton_6

TextButton_7.Parent = HL
TextButton_7.BackgroundColor3 = Color3.new(0.196078, 0.196078, 0.196078)
TextButton_7.BorderColor3 = Color3.new(0, 0, 0)
TextButton_7.BorderSizePixel = 0
TextButton_7.Position = UDim2.new(0.0800027028, 0, 0.797785342, 0)
TextButton_7.Size = UDim2.new(0, 118, 0, 28)
TextButton_7.Font = Enum.Font.Jura
TextButton_7.Text = "Speed Up"
TextButton_7.TextColor3 = Color3.new(1, 1, 1)
TextButton_7.TextSize = 19
TextButton_7.TextWrapped = true
TextButton_7.MouseButton1Down:Connect(function()
	game.Workspace.xXDonaldDuck77Xx.Humanoid.WalkSpeed = 50
end)
UICorner_10.Parent = TextButton_7
