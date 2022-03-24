while wait(1) do
    for _, v in pairs(game.Players:GetPlayers()) do
        for _, v2 in pairs(v.Character:GetChildren()) do
            if v2:IsA("Tool") then
                if v2.Handle:FindFirstChild("Sound") then
                    local Sound = v2.Handle:FindFirstChild("Sound")
                    Sound.TimePosition = math.random(0, 100)
                end
            end
        end
        for _, v3 in pairs(v.Backpack:GetChildren()) do
            if v3:IsA("Tool") then
                if v3.Handle:FindFirstChild("Sound") then
                    local Sound = v3.Handle:FindFirstChild("Sound")
                    Sound.TimePosition = math.random(0, 100)
                end
            end
        end
    end
end