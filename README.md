# SF-UI-Library (OPEN SOURCE SO YOU CANT SAY ITS VIRUS)
An normal ui library made by not_void.dev.

--example window
local gui = field:NewGUI({
	UIName = "example";
})

--example tab
local tab = gui:CreateTab({
	TabName = "aaa";
	Image = nil
})

--example button
local button = tab:CreateButton({
	ButtonName = 'print test';
	Callback = function()
		print('test')
	end,
})

--example textbox
local textbox = tab:CreateTextBox({
	Name = 'testbox'
	--funfact you get the textbox's text using: textbox:GetText() -- this will return the text in the box
})

--example button a
local buttong = tab:CreateButton({
	ButtonName = 'print textbox';
	Callback = function()
		print(textbox:GetText()) -- this will return the text in the box
	end,
})


--example label
local label = tab:CreateLabel({
	Name = "test label";
	Description = "in the feature it will allow more text :("
})

--example label
local warning = tab:CreateWarning({
	Name = "test warning";
	Description = "in the feature it will allow more text :("
})

--example switch
local switch = tab:CreateSwitch({
	Name = "test warning";
	Callback = function(v)
		print(v)
	end,
})

-- slider will be in the feature!
