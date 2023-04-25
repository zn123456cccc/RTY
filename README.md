local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "blackhub", HidePremium = false, lntroText = "Goldenhub", SaveConfig = true, ConfigFolder = "OrionTest"})

local Tab = Window:MakeTab({

	Name = "ผลักมีประโยชน์",	Icon = "rbxassetid://4483345998",

	PremiumOnly = false

})

OrionLib:MakeNotification({

	Name = "",

	Content = "ขอให้สนุก🥰",

	Image = "rbxassetid://4483345998",

	Time = 5

})

Tab:AddButton({

	Name = "กดปุ่มเดียวจบ",

	Callback = function()

      	Section:NewToggle("InfCharge", "", function(v)

_G.InfCharge = v

end)

Section:NewToggle("InfEnergy", "", function(v)

_G.InfEnergy = v

end)

Section:NewToggle("No Cooldown", "", function(v)

_G.Nocooldown = v

end)

  	end    

})

OrionLib:Init()
