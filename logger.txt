-- stiizzy cat was here

local DecalLogger = Instance.new("ScreenGui")
local Topbar = Instance.new("Frame")
local Executor = Instance.new("Frame")
local Logem = Instance.new("TextButton")
local clearconsole = Instance.new("TextButton")
local Logs = Instance.new("TextBox")
local copyid = Instance.new("TextButton")
local savetotxt = Instance.new("TextButton")
local Cum = Instance.new("TextButton")
local Title = Instance.new("TextLabel")
local Title_2 = Instance.new("TextLabel")

--Properties:

DecalLogger.Name = "DecalLogger"
DecalLogger.Parent = game.CoreGui
DecalLogger.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
DecalLogger.ResetOnSpawn = false

Topbar.Name = "Topbar"
Topbar.Parent = DecalLogger
Topbar.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
Topbar.BorderSizePixel = 0
Topbar.Position = UDim2.new(0.310107589, 340, 0.253102034, 165)
Topbar.Size = UDim2.new(0, 415, 0, 24)

Executor.Name = "Executor"
Executor.Parent = Topbar
Executor.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Executor.BorderSizePixel = 0
Executor.Position = UDim2.new(0, 0, 1, 0)
Executor.Size = UDim2.new(0, 415, 0, 222)

Logem.Name = "Logem"
Logem.Parent = Executor
Logem.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
Logem.BorderSizePixel = 0
Logem.Position = UDim2.new(0.036144577, 0, 0.810810804, 0)
Logem.Size = UDim2.new(0, 82, 0, 26)
Logem.Font = Enum.Font.SourceSansBold
Logem.Text = "Log Decals"
Logem.TextColor3 = Color3.fromRGB(255, 255, 255)
Logem.TextSize = 14.000

clearconsole.Name = "clearconsole"
clearconsole.Parent = Executor
clearconsole.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
clearconsole.BorderSizePixel = 0
clearconsole.Position = UDim2.new(0.277108431, 0, 0.810810804, 0)
clearconsole.Size = UDim2.new(0, 82, 0, 26)
clearconsole.Font = Enum.Font.SourceSansBold
clearconsole.Text = "Clear Console"
clearconsole.TextColor3 = Color3.fromRGB(255, 255, 255)
clearconsole.TextSize = 14.000

Logs.Name = "Logs"
Logs.Parent = Executor
Logs.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
Logs.BorderSizePixel = 0
Logs.Position = UDim2.new(0.0216867477, 0, 0.0450450443, 0)
Logs.Size = UDim2.new(0, 399, 0, 158)
Logs.Font = Enum.Font.SourceSans
Logs.Text = ""
Logs.TextColor3 = Color3.fromRGB(255, 255, 255)
Logs.TextSize = 14.000

copyid.Name = "copyid"
copyid.Parent = Executor
copyid.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
copyid.BorderSizePixel = 0
copyid.Position = UDim2.new(0.510843396, 0, 0.810810804, 0)
copyid.Size = UDim2.new(0, 82, 0, 26)
copyid.Font = Enum.Font.SourceSansBold
copyid.Text = "Copy Id"
copyid.TextColor3 = Color3.fromRGB(255, 255, 255)
copyid.TextSize = 14.000

savetotxt.Name = "savetotxt"
savetotxt.Parent = Executor
savetotxt.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
savetotxt.BorderSizePixel = 0
savetotxt.Position = UDim2.new(0.756626487, 0, 0.810810804, 0)
savetotxt.Size = UDim2.new(0, 82, 0, 26)
savetotxt.Font = Enum.Font.SourceSansBold
savetotxt.Text = "Save To Txt"
savetotxt.TextColor3 = Color3.fromRGB(255, 255, 255)
savetotxt.TextSize = 14.000

Cum.Name = "Cum"
Cum.Parent = Topbar
Cum.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Cum.BackgroundTransparency = 1.000
Cum.BorderSizePixel = 0
Cum.Position = UDim2.new(0.930438995, 0, 0, 0)
Cum.Size = UDim2.new(0, 28, 0, 24)
Cum.Font = Enum.Font.SourceSansItalic
Cum.Text = "-"
Cum.TextColor3 = Color3.fromRGB(255, 255, 255)
Cum.TextSize = 35.000
Cum.TextWrapped = true

Title.Name = "Title"
Title.Parent = Topbar
Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Title.BackgroundTransparency = 1.000
Title.BorderSizePixel = 0
Title.Position = UDim2.new(-0.0502793305, 0, 0, 0)
Title.Size = UDim2.new(0, 177, 0, 24)
Title.Font = Enum.Font.SourceSansBold
Title.Text = "Decal Logger"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextScaled = true
Title.TextSize = 14.000
Title.TextWrapped = true

Title_2.Name = "Title"
Title_2.Parent = Topbar
Title_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Title_2.BackgroundTransparency = 1.000
Title_2.BorderSizePixel = 0
Title_2.Position = UDim2.new(0.294298977, 0, 0.458333343, 0)
Title_2.Size = UDim2.new(0, 40, 0, 12)
Title_2.Font = Enum.Font.SourceSansBold
Title_2.Text = "v1.1"
Title_2.TextColor3 = Color3.fromRGB(255, 255, 255)
Title_2.TextSize = 14.000
Title_2.TextWrapped = true

-- Scripts:

local function LMNZHDF_fake_script() -- Topbar.LocalScript 
	local script = Instance.new('LocalScript', Topbar)

	function Tween(Object, Time, Customization)
		game:GetService("TweenService"):Create(Object, TweenInfo.new(Time), Customization):Play()
	end
	
	
	-- Tweening.
	local Cumm = script.Parent.Cum
	local MainUI = script.Parent
	local Executor = MainUI.Executor
	local clear = script.Parent.Executor.clearconsole
	local Logg = script.Parent.Executor.Logem
	local console = script.Parent.Executor.Logs
	local copy = script.Parent.Executor.copyid
	local save = script.Parent.Executor.savetotxt
	local CloseDis = true
	local MiniDis = true
	
	Cumm.MouseButton1Click:Connect(function()
		if MiniDis == true then do
				--Executor.Visible = false
				for i,v in pairs(script.Parent.Executor:GetChildren()) do
					if v:IsA("TextButton") then
						v.Visible = false
					end
				end
				for i,v in pairs(script.Parent.Executor:GetChildren()) do
					if v:IsA("TextBox") then
						v.Visible = false
					end
				end
				wait(.25)
				Tween(script.Parent.Executor, .35, {Size = UDim2.new(0, 415,0, 0)})
				Cumm.Text = "+"
				wait(.35)
				MiniDis = false
			end
		else
			wait(.25)
			Tween(script.Parent.Executor, .35, {Size = UDim2.new(0, 415,0, 222)})
			for i,v in pairs(script.Parent.Executor:GetChildren()) do
				if v:IsA("TextButton") then
					v.Visible = true
				end
			end
			for i,v in pairs(script.Parent.Executor:GetChildren()) do
				if v:IsA("TextBox") then
					v.Visible = true
				end
			end
			Cumm.Text = "-"
			wait(.35)
			MiniDis = true
		end
	end)
	clear.MouseButton1Click:Connect(function()
		console.Text = " "
	end)
	
	Logg.MouseButton1Click:Connect(function()
		local plrs = game:GetService("Players")
		for _,v in next, plrs:GetPlayers() do
			for _,b in next, workspace:GetChildren() do
				if b.Name == v.Name .. "Spray" then
					script.Parent.Executor.Logs.Text = "Spray detected: ".. b.Decal.Texture..":)"
				end
			end
		end
	end)
	copy.MouseButton1Click:Connect(function()
     setclipboard(Logs.text) 
	end)
	save.MouseButton1Click:Connect(function()
		writefile("LoggedDecalId.txt", Logs.text )
	end)
	
	
	
end
coroutine.wrap(LMNZHDF_fake_script)()
local function XCVSB_fake_script() -- Topbar.Drag 
	local script = Instance.new('LocalScript', Topbar)

	local a=game:GetService("UserInputService")function drag(b)dragToggle=nil dragSpeed=0.23 dragInput=nil dragStart=nil dragPos=nil function updateInput(a)Delta=a.Position-dragStart Position=UDim2.new(startPos.X.Scale,startPos.X.Offset+Delta.X,startPos.Y.Scale,startPos.Y.Offset+Delta.Y)game:GetService("TweenService"):Create(b,TweenInfo.new(0.25),{Position=Position}):Play()end b.InputBegan:Connect(function(c)if(c.UserInputType==Enum.UserInputType.MouseButton1 or c.UserInputType==Enum.UserInputType.Touch)and a:GetFocusedTextBox()==nil then dragToggle=true dragStart=c.Position startPos=b.Position c.Changed:Connect(function()if c.UserInputState==Enum.UserInputState.End then dragToggle=false end end)end end)b.InputChanged:Connect(function(a)if a.UserInputType==Enum.UserInputType.MouseMovement or a.UserInputType==Enum.UserInputType.Touch then dragInput=a end end)game:GetService("UserInputService").InputChanged:Connect(function(a)if a==dragInput and dragToggle then updateInput(a)end end)end drag(script.Parent)
end
coroutine.wrap(XCVSB_fake_script)()
