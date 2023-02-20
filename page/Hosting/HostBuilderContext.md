``` csharp
public class HostBuilderContext
{
    public HostBuilderContext(IDictionary<object, object> properties)
    {
        Properties = properties ?? throw new System.ArgumentNullException(nameof(properties));
    }

    public IHostEnvironment HostingEnvironment { get; set; }

    public IConfiguration Configuration { get; set; }

    public IDictionary<object, object> Properties { get; }
}
```
