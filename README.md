local DiscordLib = loadstring(game:HttpGet"https://pastebin.com/raw/XMBepAJH")()

local win = DiscordLib:Window("Blacky Hub")

local serv = win:Server("A 0nepiece Game", "")
local AutoFram = serv:Channel("Main")
 Times = AutoFram:Label("Server Time")
 local function UpdateTime()
 local GameTime = math.floor(workspace.DistributedGameTime+0.5)
 local Hour = math.floor(GameTime/(60^2))%24
 local Minute = math.floor(GameTime/(60^1))%60
 local Second = math.floor(GameTime/(60^0))%60
 Times:Refresh("Hour : "..Hour.." Minute : "..Minute.." Second : "..Second)
 end
 spawn(function()
 while true do
 UpdateTime()
 game:GetService("RunService").RenderStepped:Wait()
 end
 end)
 Time = AutoFram:Label("Client")
 local function UpdateTime()
 local GameTime = math.floor(workspace.DistributedGameTime+0.5)
 
 local Ping = game:GetService("Stats").Network.ServerStatsItem["Data Ping"]:GetValueString()
 local Fps = (workspace:GetRealPhysicsFPS())
 Time:Refresh("Fps :"..Fps.."Ping :"..Ping)
 end
 spawn(function()
 while true do
 UpdateTime()
 game:GetService("RunService").RenderStepped:Wait()
 end
 end)
 AutoFram:Seperator()
 AutoFram:Label("------- AutoFarm Crocodile -------")
 AutoFram:Button("Quest Giver",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(4, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-107.7640380859375, -56.592552185058594, 6833.34228515625)}):Play()
end)
 AutoFram:Toggle("Auto Farm Crocodile ",false,function(bool)
 _G.asdada = bool
 end)
spawn(function()
    while wait() do
        if _G.asdada then
            pcall(function()
local args = {
    [1] = "Devil Fruit",
    [2] = "Q",
    [3] = CFrame.new(291.128662109375, -55.60483932495117, 7665.642578125) * CFrame.Angles(-0.5612145662307739, 0.1254674792289734, 0.07850577682256699),
    [4] = workspace.Entities.Crocodile.Torso,
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))
           end)
         end
     end
end)
AutoFram:Toggle("Auto TP Crocodile",false,function(bool)
    _G.croc = bool
end)
spawn(function()
    while wait() do
        if _G.croc then
            pcall(function()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0.1, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(326.33203125, 82.65784454345703, 7907.81689453125)}):Play()
           end)
         end
     end
end)
AutoFram:Seperator()
AutoFram:Label("------- AutoFarm Akainu -------")
AutoFram:Seperator()
AutoFram:Button("Quest Giver",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(4), 
{CFrame = CFrame.new(8884.7001953125, -44.713706970214844, -2211.007568359375)}):Play()
end)
AutoFram:Toggle("Auto Farm Akainu ",false,function(bool)
 _G.banedit = bool
 end)
spawn(function()
    while wait() do
        if _G.banedit then
            pcall(function()
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Devil Fruit",
    [2] = "Q",
    [3] = CFrame.new(9738.34765625, -45.53757095336914, -1738.15283203125) * CFrame.Angles(-2.3808228969573975, 0.8969035148620605, 2.50205397605896),
    [4] = workspace.Entities.Akainu:FindFirstChild("Akainu Cloak"),
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

           end)
         end
     end
end)
AutoFram:Toggle("Auto TP Akainu",false,function(bool)
    _G.aka = bool
end)
spawn(function()
    while wait() do
        if _G.aka then
            pcall(function()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0.1, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(9970.61328125, 71.179931640625, -1868.1650390625)}):Play()
           end)
         end
     end
end)
AutoFram:Seperator()
AutoFram:Label("------- AutoFarm Caesar -------")
AutoFram:Button("Quest Giver",function()
   local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(4, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(8884.7001953125, -44.713706970214844, -2211.007568359375)}):Play()
end)
AutoFram:Toggle("Auto Caesar",false,function(bool)
_G.Caesarsa = bool
end)
spawn(function()
   while wait() do
      if _G.Caesarsa then 
           pcall(function()
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Devil Fruit",
    [2] = "Q",
    [3] = CFrame.new(9530.466796875, 31.79717254638672, -2352.4541015625) * CFrame.Angles(-2.020193338394165, -0.7869186997413635, -2.1686954498291016),
    [4] = workspace.Map.Islands:FindFirstChild("Punk Hazard").Model:FindFirstChild("Punk Hazard").Part,
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

          end)
        end
    end
end)
AutoFram:Toggle("Auto TP Caesar",false,function(bool)
   _G.css = bool
end)
spawn(function()
   while wait() do
       if _G.css then
           pcall(function()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0.1, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(9358.341796875, 160.5977020263672, -2429.226806640625)}):Play()
          end)
        end
    end
end)
AutoFram:Seperator()
AutoFram:Label("------- AutoFarm Doflamingo -------")
AutoFram:Button("Quest Giver",function()
   local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(4, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(6609.43896484375, -34.35888671875, 1481.6842041015625)}):Play()
end)
AutoFram:Toggle("Auto Doflamingo",false,function(bool)
_G.Dofa = bool
end)
spawn(function()
   while wait() do 
      if _G.Dofa then 
           pcall(function()
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Devil Fruit",
    [2] = "Q",
    [3] = CFrame.new(6949.5478515625, -17.838851928710938, 1383.6541748046875) * CFrame.Angles(-0.47966137528419495, -0.3493269383907318, -0.17619363963603973),
    [4] = workspace.Map.Islands:FindFirstChild("Flamingo's Island").Model:FindFirstChild("Flamingo's Island"):FindFirstChild("Buggyhouse.2").Model.Part,
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

          end)
        end
    end
end)
AutoFram:Toggle("Auto TP Doflamingo",false,function(bool)
   _G.cess = bool
end)
spawn(function()
   while wait() do
       if _G.cess then
           pcall(function()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0.1, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(6883.41015625, 50.45216369628906, 1551.629150390625)}):Play()
          end)
        end
    end
end)
AutoFram:Seperator()
AutoFram:Label("------- AutoFarm Marco -------")
AutoFram:Button("Quest Giver",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(4), 
{CFrame = CFrame.new(3008.46533203125, -56.859169006347656, 1225.415771484375)}):Play()
end)
AutoFram:Toggle("Auto Farm Marco ",false,function(bool)
 _G.bandit = bool
 end)
spawn(function()
    while wait() do
        if _G.bandit then
            pcall(function()
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Devil Fruit",
    [2] = "Q",
    [3] = CFrame.new(2594.170654296875, 91.03683471679688, 1077.0047607421875) * CFrame.Angles(-2.4907095432281494, 0.3454592823982239, 2.889193296432495),
    [4] = workspace.Entities.Marco:FindFirstChild("Right Leg"),
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

           end)
         end
     end
end)
spawn(function()
    while wait() do
        if _G.bandit then
            pcall(function()
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Devil Fruit",
    [2] = "F",
    [3] = CFrame.new(2595.452392578125, 89.44569396972656, 1073.610107421875) * CFrame.Angles(-2.4743216037750244, 0.3439044654369354, 2.8819618225097656),
    [4] = workspace.Map.Islands:FindFirstChild("Phoenix Nest").Model:FindFirstChild("Marco island"):FindFirstChild("Meshes/marconew.2 (2)"),
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

           end)
         end
     end
end)
AutoFram:Toggle("Auto TP Marco",false,function(bool)
    _G.MARCO = bool
end)
spawn(function()
    while wait() do
        if _G.MARCO then
            pcall(function()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0.5, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(2658.96435546875, 190.01609802246094, 932.05517578125)}):Play()
           end)
         end
     end
end)
AutoFram:Seperator()
 AutoFram:Label("------- AutoFarm Katakuri -------")
 AutoFram:Button("Quest Giver",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(4, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(3008.46533203125, -56.859169006347656, 1225.415771484375)}):Play()
end)
AutoFram:Toggle("Auto Katakuri",false,function(bool)
_G.Katakuri = bool
end)
spawn(function()
    while wait() do
       if _G.Katakuri then 
            pcall(function()
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Devil Fruit",
    [2] = "Q",
    [3] = CFrame.new(2811.375, 47.14144515991211, 1043.0845947265625) * CFrame.Angles(-0.7939582467079163, -0.05789569020271301, -0.05879472196102142),
    [4] = workspace.Map.Islands:FindFirstChild("Phoenix Nest").Model:FindFirstChild("Marco island"):FindFirstChild("Meshes/SM_Env_GrassPatch_02"),
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))
 
           end)
         end
     end
end)
AutoFram:Toggle("Auto TP Katakuri",false,function(bool)
    _G.aTP = bool
end)
spawn(function()
    while wait() do
        if _G.aTP then
            pcall(function()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0.1, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(2770.9736328125, 142.89849853515625, 1172.615234375)}):Play()
           end)
         end
     end
end)
AutoFram:Seperator()
 AutoFram:Label("------- Auto Skill -------")
AutoFram:Toggle("Auto Boost + Buso ",false,function(bool)

    game.Players.localPlayer.Character.Humanoid.Health = 0
end)
spawn(function()
    while wait() do
       if game.Players.localPlayer.Character.Humanoid.Health  == 0 then 
            pcall(function()
wait(15)
-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Fighting Style",
    [2] = "F",
    [3] = CFrame.new(2915.448486328125, -59.859153747558594, 1306.1949462890625) * CFrame.Angles(-2.676845073699951, 0.21427179872989655, 3.035383462905884),
    [4] = workspace.Map.Islands:FindFirstChild("Phoenix Nest").Model:FindFirstChild("Marco island").Part,
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

           end)
         end
     end
end)

spawn(function()
    while wait() do
       if game.Players.localPlayer.Character.Humanoid.Health  == 0 then 
            pcall(function()
wait(20)
-- Script generated by SimpleSpy - credits to exx#9394

-- Script generated by SimpleSpy - credits to exx#9394

local args = {
    [1] = "Fighting Style",
    [2] = "G",
    [3] = CFrame.new(2921.24560546875, -54.03282165527344, 1289.605712890625) * CFrame.Angles(3.078249216079712, -0.12238194793462753, 3.133849620819092),
    [4] = workspace.Map.Islands:FindFirstChild("Phoenix Nest").Model.Spawner.Crystal,
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))

           end)
         end
     end
end)
AutoFram:Toggle("Auto Ken",false,function(bool)
_G.Ken = bool
end)
spawn(function()
    while wait() do
       if _G.Ken then 
            pcall(function()
            
local args = {
    [1] = "Fighting Style",
    [2] = "T",
    [3] = CFrame.new(2665.558349609375, 188.60247802734375, 933.1865844726562) * CFrame.Angles(-2.1234853267669678, -0.9036821126937866, -2.236407995223999),
    [4] = workspace.Map.Islands:FindFirstChild("Phoenix Nest").Model:FindFirstChild("Marco island"):FindFirstChild("Meshes/marconew.6 (2)"),
    [5] = 5
}

game:GetService("ReplicatedStorage").Remotes.requestAbility:FireServer(unpack(args))
     
           end)
         end
     end
end)
AutoFram:Seperator()
 AutoFram:Label("------- Notification -------")
 AutoFram:Toggle("Golden Hook Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Golden Hook") then
		HaveGoldenHook = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Golden Hook") then
		HaveGoldenHook = true
	end
	if HaveGoldenHook and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got  Golden Hook !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Golden Hook !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Doflamingo Cape Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Flamingo Cape") then
		HaveFlamingoCape = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Horns") then
		HaveFlamingoCape = true
	end
	if HaveFlamingoCape and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got Doflamingo Cape !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Doflamingo Cape !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Caesar Horns Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Horns") then
		HaveHorns = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Horns") then
		HaveHorns = true
	end
	if HaveHorns and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got Caesar Horns !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Caesar Horns !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Marine Cape Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Marine Cape") then
		HaveMarineCape = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Marine Cape") then
		HaveMarineCape = true
	end
	if HaveMarineCape and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got Mairine Cape !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Marine Cape !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Phoenix Scroll Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Phoenix Scroll") then
		HavePhoenixScroll = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Phoenix Scroll") then
		HavePhoenixScroll = true
	end
	if HavePhoenixScroll and Bool == true then
	    DiscordLib:Notification("Notification", "!! You Got Phoenix Scroll !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Phoenix Scroll !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Katakuri Trident Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Mogura") then
		HaveMogura = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Mogura") then
		HaveMogura = true
	end
	if HaveMogura and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got Katakuri Trident !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Katakuri Trident !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Mochi Fruit Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Mochi Fruit") then
		HaveMochiFruit = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Mochi Fruit") then
		HaveMochiFruit = true
	end
	if HaveMochiFruit and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got Mochi Fruit !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Mochi Fruit !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Toggle("Katakuri Scarf Notification",false,function(v)
	Bool = v
	if game.Players.LocalPlayer.Backpack:FindFirstChild("Candy Scarf") then
		HaveCandyScarf = true
	elseif game.Players.LocalPlayer.Character:FindFirstChild("Candy Scarf") then
		HaveCandyScarf = true
	end
	if HaveCandyScarf and Bool == true then
        DiscordLib:Notification("Notification", "!! You Got Candy Scarf !!", "Wow !")
		while wait() do 
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "You Get Katakuri Scarf !!",
                                        Icon = "",
                                        Duration = 3
                                    })
end
end
end)
AutoFram:Seperator()
local TP = serv:Channel("Island")
TP:Button("Stop Tween",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(0, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)}):Play()
end)
TP:Seperator()
TP:Label("------ Island ------")
TP:Button("Phoenix Nest",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(3008.46533203125, -56.859169006347656, 1225.415771484375)}):Play()
end)
TP:Button("Starter Island",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(278.6219482421875, -50.64528274536133, -212.58203125)}):Play()
end)
TP:Button("Wilderness",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-456.3139953613281, -57.10584259033203, 3046.732666015625)}):Play()
end)
TP:Button("Arena",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(4881.44287109375, -24.531841278076172, -6226.92626953125)}):Play()
end)
TP:Button("Arlong Park",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(2371.4951171875, -58.57895278930664, -915.6734619140625)}):Play()
end)
TP:Button("Desert Island",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-400.81549072265625, -56.185489654541016, 7009.05126953125)}):Play()
end)
TP:Button("Logue Town",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-3936.0283203125, -49.21131134033203, 810.3729248046875)}):Play()
end)
TP:Button("Orange Town",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(1502.439208984375, -58.814998626708984, 2878.705322265625)}):Play()
end)
TP:Button("Shell Town",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(5596.21875, -52.28487014770508, -3518.51123046875)}):Play()
end)
TP:Button("Skypiea",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(1332.5419921875, 7150.263671875, 1648.3890380859375)}):Play()
end)
TP:Button("Marine Ford",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-479.6522216796875, -0.3241960108280182, -4119.2685546875)}):Play()
end)
TP:Button("Usopp Village",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-2243.65673828125, 6.175459384918213, -7700.79541015625)}):Play()
end)
TP:Button("Impel down",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(1892.109130859375, -51.68156051635742, -3725.058837890625)}):Play()
end)
TP:Button("Flamingo Island",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(6244.95263671875, -52.49989700317383, 1492.01904296875)}):Play()
end)
TP:Button("Luffy Island",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(1820.8629150390625, -50.127830505371094, -8214.810546875)}):Play()
end)
TP:Button("Ice Island",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(-1217.64404296875, -60.70600128173828, 310.6053466796875)}):Play()
end)
TP:Button("Hot & Cold Island",function()
    local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(7, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = CFrame.new(8810.888671875, -44.71370315551758, -2347.32861328125)}):Play()
end)
local misc = serv:Channel("Setting")
misc:Button("Made By BLXCKY#1101",function()
		                                        game.StarterGui:SetCore("SendNotification", {
                                        Title = "Blacky Notification", 
                                        Text = "Thank For Using Brother!",
                                        Icon = "",
                                        Duration = 3
                                    })

end)
misc:Seperator()
misc:Label("----- System -----")
misc:Toggle("Anit AFK",true,function(vu)
    print("Anit AFK Start")
    local vu = game:GetService("VirtualUser")
    game:GetService("Players").LocalPlayer.Idled:connect(function()
    vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
    wait(1)
    vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
    end)
    end)
misc:Button("Switch Server",function()
     local PlaceID = game.PlaceId
        local AllIDs = {}
        local foundAnything = ""
        local actualHour = os.date("!*t").hour
        local Deleted = false
        function TPReturner()
            local Site;
            if foundAnything == "" then
                Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
            else
                Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
            end
            local ID = ""
            if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
                foundAnything = Site.nextPageCursor
            end
            local num = 0;
            for i,v in pairs(Site.data) do
                local Possible = true
                ID = tostring(v.id)
                if tonumber(v.maxPlayers) > tonumber(v.playing) then
                    for _,Existing in pairs(AllIDs) do
                        if num ~= 0 then
                            if ID == tostring(Existing) then
                                Possible = false
                            end
                        else
                            if tonumber(actualHour) ~= tonumber(Existing) then
                                local delFile = pcall(function()
                                    -- delfile("NotSameServers.json")
                                    AllIDs = {}
                                    table.insert(AllIDs, actualHour)
                                end)
                            end
                        end
                        num = num + 1
                    end
                    if Possible == true then
                        table.insert(AllIDs, ID)
                        wait()
                        pcall(function()
                            -- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
                            wait()
                            game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
                        end)
                        wait(.1)
                    end
                end
            end
        end
        function Teleport() 
            while wait() do
                pcall(function()
                    TPReturner()
                    if foundAnything ~= "" then
                        TPReturner()
                    end
                end)
            end
        end
        Teleport()

end)
misc:Button("Rejoin Server",function()
    local ts = game:GetService("TeleportService") local p = game.Players.LocalPlayer ts:Teleport(game.PlaceId, p) 
end)
misc:Label()
