function createESP(player)
    local highlight = Instance.new("Highlight")
    highlight.Parent = player.Character
    highlight.Adornee = player.Character
    highlight.FillColor = Color3.new(1, 0, 0) -- Cor vermelha
    highlight.OutlineColor = Color3.new(1, 1, 1) -- Cor branca
end
for _, player in pairs(game.Players:GetPlayers()) do
    if player ~= game.Players.LocalPlayer and player.Character then
        createESP(player)
    end
end
game.Players.PlayerAdded:Connect(function(player)
    player.CharacterAdded:Connect(function()
        createESP(player)
    end)
end)
function tradeScam(targetPlayer)
    -- Código para realizar o Trade Scam
    -- Nota: Este tipo de script é contra os termos de serviço do Roblox e pode resultar em banimento.
end
function tradeFreeze(targetPlayer)
    -- Código para congelar a troca
    -- Nota: Este tipo de script é contra os termos de serviço do Roblox e pode resultar em banimento.
end
local targetPlayer = game.Players:FindFirstChild("NomeDoJogadorAlvo")
if targetPlayer then
    tradeScam(targetPlayer)
    tradeFreeze(targetPlayer)
end
