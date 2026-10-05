ls -la - can see who has read write execute permissions (extend version of ls)
Example of ls -la: drwxr-xr-x  2 kali kali 4096 Sep 29 10:00 Desktop : (here 'd' — this is a directory (a '-' here means it's a regular file) : rwxr-xr-x  permissions, in three groups of three: owner (rwx = read/write/execute), group (r-x), others (r-x) : kali kali — owner, then group : 4096 — size in bytes : Sep 29 10:00 — last modified : Desktop — the name
rwx each have value: 4+2+1
So when we want to give owner or group or others some permission, we can simply add or minus numbers according to their value.
chmod 700 test.txt - owner gets full access, nobody else gets any
chmod 644 test.txt - owner read/write, everyone else read-only
chmod 755 text.txt - owner has all access (rwx = 7), group has read and execute (r-x = 5), others can read and execute (r-x = 5)
#Another way:
u: User / Owner, g: Group, o: Others, a: All, r: Read, w: Write, x: Execute
chmod a+x script.txt - Grant execute access to everyone
chmod go-w text.txt - Remove write access from group and others
chmod +x texting.txt - gives all execute permission to this file
