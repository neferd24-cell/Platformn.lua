local button = script.Parent
local platform = workspace:WaitForChild("Platform")

button.Text = "Mostrar plataforma"

button.MouseButton1Click:Connect(function()
    if platform.Transparency == 1 then
        platform.Transparency = 0
        platform.CanCollide = true
        button.Text = "Ocultar plataforma"
    else
        platform.Transparency = 1
        platform.CanCollide = false
        button.Text = "Mostrar plataforma"
    end
end
