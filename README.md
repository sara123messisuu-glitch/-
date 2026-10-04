-- 1. استدعاء مكتبة Orion UI
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/shlexcc/Orion/main/source"))()

-- 2. إنشاء النافذة
local Window = Library:CreateWindow({
    Title = "My First Hack ⚡", 
    Description = "تعلم صناعة السكربتات", 
    DefaultFolder = "MyHub"
})

-- 3. إنشاء تبويب
local Tab = Window:CreateTab({
    Name = "اللاعب",
    Icon = "rbxassetid://4483362458"
})

-- 4. إضافة زر لتغيير السرعة
Tab:AddButton({
    Name = "سرعة فائقة (Speed Hack)",
    Callback = function()
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 100
    end
})

-- 5. تشغيل المكتبة
Library:Init()
