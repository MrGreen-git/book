```csharp
public static class Host
{
	public static IHostBuilder CreateDefaultBuilder() =>
		CreateDefaultBuilder(args: null);

	public static IHostBuilder CreateDefaultBuilder(string[] args)
	{
		HostBuilder builder = new();
		return builder.ConfigureDefaults(args);
	}
}
```
