# Assorted C# Notes
- If you need to create your own Main() to test your own methods w/o a code runner...
  - add ```<GenerateProgramFile>false</GenerateProgramFile>``` to filename.csproj in a ```<PropertyGroup>
    - The tests auto generate a Main() that causes a "multiple entry point" error.
    - This prevents the the Main() from being generated
      - Oddly Enough, it still runs the tests just fine when using dotnet test
