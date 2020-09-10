# Leak report

_Functions strip, is_cleaned, and main uses a variable that doesn't relinquish memory. After looking, is_cleaned used a variable from strip that it doesn't let go. So I had to make sure that it doesn't release memory with an empty string, but I altered it so it free's memory after it is done using it.__
