-- Made by Lyvali
-- Ty for using!!

local bypassLoad = false

if bypassLoad == true then
	return
end

pcall(function() bypassLoad = true end)

if not game:IsLoaded() then game.Loaded:Wait() end

local ChatService = game:GetService("TextChatService")
local TweenService = game:GetService("TweenService")
local UserInputService = game:GetService("UserInputService")
local isNew = false

local ChatMessage = "[🎀] This chat "..string.reverse("ssapyb").." was made by Lyvali"

local function checkChatVersion()
	local new = Enum.ChatVersion.TextChatService
	local old = Enum.ChatVersion.LegacyChatService

	if ChatService.ChatVersion == new then
		return isNew == true
	elseif ChatService.ChatVersion == old then
		return isNew == false
	end
end

local function dragGUI(gui)
	task.spawn(function()
		local dragging
		local dragInput
		local dragStart = Vector3.new(0,0,0)
		local startPos
		local function update(input)
			local delta = input.Position - dragStart
			local Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
			TweenService:Create(gui, TweenInfo.new(.20), {Position = Position}):Play()
		end
		gui.InputBegan:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
				dragging = true
				dragStart = input.Position
				startPos = gui.Position

				input.Changed:Connect(function()
					if input.UserInputState == Enum.UserInputState.End then
						dragging = false
					end
				end)
			end
		end)
		gui.InputChanged:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
				dragInput = input
			end
		end)
		UserInputService.InputChanged:Connect(function(input)
			if input == dragInput and dragging then
				update(input)
			end
		end)
	end)
end

if checkChatVersion() == (isNew == true) then
	ChatService.TextChannels.RBXGeneral:SendAsync(ChatMessage)
elseif checkChatVersion() == (isNew == false) then
	game.ReplicatedStorage.DefaultChatSystemChatEvents.SayMessageRequest:FireServer(ChatMessage, "All")
end

local LyvaliUI = Instance.new("ScreenGui")
local ChatBypasser = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local Message = Instance.new("TextBox")
local UICorner_2 = Instance.new("UICorner")
local Send = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")

local prnt = nil
local COREGUI = game:GetService("CoreGui")

LyvaliUI.Name = "LyvaliUI"
LyvaliUI.Parent = COREGUI.RobloxGui
LyvaliUI.DisplayOrder = 9e909

--syn.protect_gui(LyvaliUI)

ChatBypasser.Name = "ChatBypasser"
ChatBypasser.Parent = LyvaliUI
ChatBypasser.AnchorPoint = Vector2.new(0.5, 0.5)
ChatBypasser.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
ChatBypasser.BorderColor3 = Color3.fromRGB(0, 0, 0)
ChatBypasser.BorderSizePixel = 0
ChatBypasser.Position = UDim2.new(0.499498487, 0, 0.896021724, 0)
ChatBypasser.Size = UDim2.new(0, 336, 0, 57)

UICorner.CornerRadius = UDim.new(1, 0)
UICorner.Parent = ChatBypasser

Message.Name = "Message"
Message.Parent = ChatBypasser
Message.AnchorPoint = Vector2.new(0.5, 0.5)
Message.BackgroundColor3 = Color3.fromRGB(15, 15, 15)
Message.BorderColor3 = Color3.fromRGB(0, 0, 0)
Message.BorderSizePixel = 0
Message.Position = UDim2.new(0.339285702, 0, 0.491228074, 0)
Message.Size = UDim2.new(0, 206, 0, 45)
Message.Font = Enum.Font.SourceSans
Message.PlaceholderText = "Message to bypass"
Message.Text = ""
Message.TextColor3 = Color3.fromRGB(255, 255, 255)
Message.TextScaled = true
Message.TextSize = 14.000
Message.TextWrapped = true

UICorner_2.CornerRadius = UDim.new(1, 0)
UICorner_2.Parent = Message

Send.Name = "Send"
Send.Parent = ChatBypasser
Send.AnchorPoint = Vector2.new(0.5, 0.5)
Send.BackgroundColor3 = Color3.fromRGB(15, 15, 15)
Send.BorderColor3 = Color3.fromRGB(0, 0, 0)
Send.BorderSizePixel = 0
Send.Position = UDim2.new(0.815476179, 0, 0.5, 0)
Send.Size = UDim2.new(0, 102, 0, 45)
Send.Font = Enum.Font.SourceSans
Send.Text = "Send"
Send.TextColor3 = Color3.fromRGB(255, 255, 255)
Send.TextScaled = true
Send.TextSize = 14.000
Send.TextWrapped = true

UICorner_3.CornerRadius = UDim.new(1, 0)
UICorner_3.Parent = Send

Send.MouseButton1Click:Connect(function()
	local unbypassedTable = { "ass", "cum", "cock", "fuck", "asshole", "rape", "boobs", "sex", "hoe", "porn", "nigga", "penis", "thot", "xxx", "hentai", "bitch", "bitches", "shit", "kys", "butthole", "masturbate", "blowjob", "cock sucker", "dumbass", "motherfucker", "sex", "pussy", "whore", "slut" }
	local bypassTable = { "â҆s҃ș҄", "с҄҄u҆҆М҄҄", "с҃҃҆о҅҅҇с҃҃κ҅҆҄", "f҄҄҃u҆҆҇с҆҄҅҅κ҅҆҄", "а҃҃s҄҃ș҄h҆҇҅о҃҇҅lе҇҆", "r҃҃҅а҇҆҆p҅҇҄҆е҇҆҆", "b҆҆҇҃҅о҇҇҆о҄҅b҃҆ș҄҄", "Ѕ҆҆҇҅҃҄҆е҇҅҅х҅҇҅", "һ҅҅҇҆о҃҄҇҅҆҆е҇҆҆", "р҄҆o҄҃҇҆҅ѓ҇҆n҃҇҆", "ŋ҇҄҅і҄҇҆ɠ҃҆҇҄҄҆g҇҄҄҆ɑ", "p҃҄҆ɐ҇҄҃҅ŋ҆҄҆i҃҇҆ʂ҅҇҄҆", "ʈ҅҃҃҆ɧ҇҇҃҆҆o҄҇҅ʈ҇҇҆", "χχχ", "ɧ҄҄҇҆ɐ҄҇҆ŋ҄҄҇҆t҄҄҇҆ɑ҃҃҆i҇҅", "ɓ҇҃҆i҄҇҆t҃҃҇҆ç҄҄҇҅҅ɧ҃", "ɓ҇҃҆i҄҇҆t҃҃҇҆ç҄҄҇҅҅ɧ҃es", "ʂ҃҃҇҅҅ɧ҇҆҃҃҅it҆҆҇҆", "ҡ҇҃҄҅҆ɣ҄҇҇҅ѕ҃҄҆", "ɓ҃҃҄҆҆ʊ҇҇҅ʈ҄҄҆t҇҇҃҆ɧ҄҄҃҆o҇҇҆l҄҄҅ɐ", "ɱ҄҄҇҅ɑ҃҇҆s҄҇҇҇҆ʈ҇҅ʊ҅҄҆ɾ҇҇҆e҄҆ɓ҄҃҇҇҆ɑ҅҅t҆҅҅ɐ҃҄҆", "ɓ҆҆l҇҅o҆҃҄҇҆ɯ҅҄҄҅҆҆҄҅ʝ҃҄҅҇҆҆o҇҇҄҆b҇҅҄҃҅", "ç҇҄҅o҇҇҄҆҅҅ç҇҆҆k҃҃҃҄҅ ҇҆ʂ҅҄҃҇҆ʊ҇҇҄҆ç҅҄҃҇҆k҇҇҆҅ɐ҇҆҆r҇҇҇҅҅", "ɖ҅҆҇҆u҄҃҇҆ɱ҄҄҇҆ɓ҃҄҅҆҆҇҃҄҅҅ɑ҇҄҆ʂ҃҄҇҆s҅҄", "ɱ҄҅҃҆o҇҆҄҅ʈɧ҇҆҆ɐ҅҃҃҃҆r҅҄҄҇҆f҇҇҄҆ʊ҃҄҅҅҇҇҆҄҆ç҃҃҇҆k҆҅ɐ҇҆r҃҄҆", "ʂ҆҅҇҅ɐ҄҃҄҇҆χ҇҇҆҅", "p҅҇҇҆ʊ҃҄҇҆s҆҄҆ʂ҇҇҇҆ɣ҄҃҃҃҅", "ɯ҄҄҅ɧ҇҇҄҆o҃҃҆҇҆ɾ҃҃҄҇҆ɐ҄҄҇҆", "ʂ҆҇҆ɭ҄҃҇҆u҇҇҄҅҆ʈ҄҇҆", "" }
	
	if checkChatVersion() == (isNew == true) then
		--ChatService.TextChannels.RBXGeneral:SendAsync(Message.Text)
		for s in string.gmatch(string.lower(Message.Text), "%S+") do
			for i, key in ipairs(unbypassedTable) do
				if s == string.lower(key) then
					s = bypassTable[i]
					break
				end
			end
			ChatService.TextChannels.RBXGeneral:SendAsync(s)
			wait(1.015242453643565346313)
		end
	elseif checkChatVersion() == (isNew == false) then
		--game.ReplicatedStorage.DefaultChatSystemChatEvents.SayMessageRequest:FireServer(Message.Text, "All")
		for s in string.gmatch(string.lower(Message.Text), "%S+") do
			for i, key in ipairs(unbypassedTable) do
				if s == string.lower(key) then
					s = bypassTable[i]
					break
				end
			end
			game.ReplicatedStorage.DefaultChatSystemChatEvents.SayMessageRequest:FireServer(s, "All")
			wait(1.015242453643565346313)
		end
	end
end)

dragGUI(ChatBypasser)
