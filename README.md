# Date Comparison

Compare a scraped date with today's date using VB functions in a Studio process.

## Disclaimer

**The contents of this repository are NOT OFFICIALLY SUPPORTED by UiPath. Anything you use is AT YOUR OWN DISCRETION.**

## Automation Steps

1. dateStringScraped is of type String and follows the format "yyyy-M-dd".

2. dateStringScraped is then converted to the type DateTime using the following function:

```vb
DateTime.ParseExact(dateStringScraped, "yyyy-M-dd", System.Globalization.CultureInfo.InvariantCulture)
```

If your dateStringScraped is of a different format, e.g. "MM/dd/yyyy", just update the formatting string in the above function.

3. dateTimeToday is created with the following function:

```vb
DateTime.Today
```

## Owner

[Michael Agarenzo](https://linkedin.com/in/magarenzo), Technical Account Manager at UiPath