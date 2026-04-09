# def convert_minutes(minutes):
    hours = minutes // 60
    mins = minutes % 60

    if hours > 0 and mins > 0:
        if hours == 1:
            return f"{hours} hr {mins} minutes"
        else:
            return f"{hours} hrs {mins} minutes"
    elif hours > 0:
        if hours == 1:
            return f"{hours} hr"
        else:
            return f"{hours} hrs"
    else:
        return f"{mins} minutes"


# Example usage
num = int(input("Enter minutes: "))
print(convert_minutes(num))
