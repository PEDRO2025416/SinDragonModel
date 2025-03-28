-- SinDragonModel Script
-- Script to create a Sin Dragon model

local ReplicatedStorage = game:GetService("ReplicatedStorage")

-- Check if the model is already in ReplicatedStorage
local existingModel = ReplicatedStorage:FindFirstChild("SinDragonModel")
if existingModel then
    return -- Exit if the model already exists
end

-- Create the Sin Dragon model
local sinDragonModel = Instance.new("Model")
sinDragonModel.Name = "SinDragonModel"
sinDragonModel.Parent = ReplicatedStorage

-- Add parts to the model (Example)
local head = Instance.new("Part")
head.Name = "Head"
head.Size = Vector3.new(4, 4, 4)
head.Position = Vector3.new(0, 10, 0)
head.Anchored = true
head.Parent = sinDragonModel

local body = Instance.new("Part")
body.Name = "Body"
body.Size = Vector3.new(6, 10, 6)
body.Position = Vector3.new(0, 5, 0)
body.Anchored = true
body.Parent = sinDragonModel

-- Add more parts, such as wings, tail, etc., depending on the model you want to create

-- Optionally, you can add accessories or custom functions here to animate or control the model

print("Sin Dragon model created and stored in ReplicatedStorage!")
