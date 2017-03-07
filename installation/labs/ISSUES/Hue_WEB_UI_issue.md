# Problem description

When Launcing Hue Web UI, an error is displayed:  bad request 400

# Explanation:

Hue considers that only IP adresses that belong to the same domain are allowed to access the Web UI, thus any other connexion (from local computer for example) is not alllowed 

# Solution:

in the Hue configuration page in Clodera Mabager, consider adding the following lines besides "" field:

[desktop]

allowed_hosts=*
