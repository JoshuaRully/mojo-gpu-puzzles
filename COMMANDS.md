# Run puzzles (remember to include your platform with -e if needed)
pixi run pXX             # NVIDIA (default) same as `pixi run -e nvidia pXX`
pixi run -e amd pXX      # AMD GPU
pixi run -e apple pXX    # Apple GPU

# Test solutions
pixi run tests           # Test all solutions
pixi run tests pXX       # Test specific puzzle

# Run manually
pixi run mojo problems/pXX/pXX.mojo     # Your implementation
pixi run mojo solutions/pXX/pXX.mojo    # Reference solution

# Interactive shell
pixi shell               # Enter environment
mojo problems/p01/p01.mojo              # Direct execution
exit                     # Leave shell

# Development
pixi run format         # Format code
pixi task list          # Available commands
