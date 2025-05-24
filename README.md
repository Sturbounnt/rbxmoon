local {insetva} = workspace:WaitForChild("partname")

script.Parent.Touched:Connect(function(hit)
	local character = hit.Parent
	if character and character:FindFirstChild("Humanoid") and character:FindFirstChild("HumanoidRootPart") then
		character:MoveTo({insetva}.Position + Vector3.new(0, 0, 0))
	end
end)
