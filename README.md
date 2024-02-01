# inet4031
with open('fileprocessor.input', 'r') as file:
    lines = file.readlines()

print("Printing out User Data:")
for line in lines:
    if line.startswith('#'):
        continue

    username, password, userid, groupid = line.strip().split(':')
    
    print(f"The user {username} has a password of {password} and has userid {userid} and groupid {groupid}")

print("End of User Data")
