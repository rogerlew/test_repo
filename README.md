<Project Sdk="Microsoft.NET.Sdk">

  <PropertyGroup>
    <TargetFramework>net6.0</TargetFramework>
    <ImplicitUsings>enable</ImplicitUsings>
    <Nullable>enable</Nullable>
  </PropertyGroup>
	
  <ItemGroup>
	<AssemblyAttribute Include="System.Runtime.CompilerServices.InternalsVisibleTo">
	  <_Parameter1>Hunter.Tests</_Parameter1>
	</AssemblyAttribute>
  </ItemGroup>

  <ItemGroup>
    <PackageReference Include="CsvHelper" Version="30.0.1" />
    <PackageReference Include="MathNet.Numerics" Version="5.0.0" />
    <PackageReference Include="Newtonsoft.Json" Version="13.0.1" />
  </ItemGroup>

  <ItemGroup>
    <ProjectReference Include="..\MessageDefLib\CommonDefLib.csproj" />
  </ItemGroup>

  <ItemGroup>
    <None Update="hunter_db\archetypes\primitives.json">
      <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
    </None>
    <None Update="hunter_db\archetypes\psfs.json">
      <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
    </None>
    <None Update="hunter_db\models\sgtr_model.json">
      <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
    </None>
    <None Update="hunter_db\procedures\rapid_shutdown.json">
      <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
    </None>
    <None Update="hunter_db\procedures\sgtr.json">
      <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
    </None>
  </ItemGroup>

</Project>
