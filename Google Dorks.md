## Searching for others Bug Bounty Programs

	inurl:bounty "reward" "scope" "report" -yeswehack -hackerone -bugcrowd -synack -openbugbounty

	"submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone" reward -site:hackerone.com

## Searching for Subdomains:

1. site:target.com
2. Remove noise w/ negative search: -site:www.target.com -inurl:news -ir
3. Keep going until we find everything

		site:tesla.com -site:www.tesla.com -shop -share

---

**site**: Tells Google to show you results from a certain site only:

	site:twitter.com

**inurl**: Searches for pages with a URL that match the search string.

	inurl:"/course/jumpto.php" site:example.com

**intitle**: Finds specific strings in a page’s title. This is useful because it allows you to find pages that contain a particular type of content.

	intitle: "index of" site:google.com

**filetype**: Searches for pages with a specific file extension. This is an incredible tool for hacking; hackers often use it to locate files on their target sites that might be sensitive, such as log and password files.

	filetype:.log site:example.com
	filetype:php intitle:"admin" site:example.com

**minus(-)**: The minus operator (-) excludes certain search results.

	"how to hack websites" -php

We can use advanced search engine options in many more ways to make your work more efficient. You can even search for the term Google search operators to discover more. These operators can be more useful than you’d expect. For example, look for all of a company’s subdomains by searching as follows:

	site:*.example.com
	site:*.api.google.com
	site:*.*.facebook.com

Look for special extensions that could indicate a sensitive file. In addition to .log, which often indicates log files, search for *.php*, *cfm*, *asp*, *.jsp*, and *.pl*, the extensions often used for script files:

	site:example.com ext:php
	site:example.com ext:log

**Or Operator**: The or operator is denoted with the pipe character (|) and can be used to search for one search term or the other, or both at the same time.

	"how to hack" site:(reddit.com | stackoverflow.com)

- **More**,

	inurl:ibm.com inurl:api 
	intitle: dashboard ext:php inurl:"&"

- **Main Dorks**

		site:*.host.com ext:asp | ext:jsp | ext:aspx | ext:jspx | ext:do | ext:action | ext:php

- **Pastebin Leaks**

		site:pastebin.com ".tesla.com" api

- **PHP extension with parameters**

		site:tesla.com ext:php inurl:?

- **API Docs**: To uncover hidden API endpoints

		inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:example.com

- **Extensions**: to find sensitive file leaks

		site:example.com ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess

- More,

		site:.*.*.nasa.gov "Server Status" | confidential | “employee only” | proprietary | top secret | classified | trade secret | internal | private

- File Upload

		(site:example[.]com | site:example[.]org) & intext:"choose file”


- Dorks for finding **admin page**

		admin1.php  
		admin1.html  
		admin2.php  
		admin2.html  
		yonetim.php  
		yonetim.html  
		yonetici.php  
		yonetici.html  
		admin/account.php  
		admin/account.html  
		admin/index.php  
		admin/index.html  
		admin/login.php  
		admin/login.html  
		admin/home.php  
		admin/controlpanel.html  
		admin/controlpanel.php  
		admin.php  
		admin.html  
		admin/cp.php  
		admin/cp.html  
		cp.php  
		cp.html  
		administrator/  
		administrator/index.html  
		administrator/index.php  
		administrator/login.html  
		administrator/login.php  
		administrator/account.html  
		administrator/account.php  
		administrator.php  
		administrator.html  
		login.html  
		modelsearch/login.php  
		moderator.php  
		moderator.html  
		moderator/login.php  
		moderator/login.html  
		moderator/admin.php  
		moderator/admin.html  
		account.php  
		account.html  
		controlpanel/  
		controlpanel.php  
		controlpanel.html  
		admincontrol.php  
		admincontrol.html  
		adminpanel.php  
		adminpanel.html  
		admin1.asp  
		admin2.asp  
		yonetim.asp  
		yonetici.asp  
		admin/account.asp  
		admin/index.asp  
		admin/login.asp  
		admin/home.asp  
		admin/controlpanel.asp  
		admin.asp  
		admin/cp.asp  
		cp.asp  
		administrator/index.asp  
		administrator/login.asp  
		administrator/account.asp  
		administrator.asp  
		login.asp  
		modelsearch/login.asp  
		moderator.asp  
		moderator/login.asp  
		moderator/admin.asp  
		account.asp  
		controlpanel.asp  
		admincontrol.asp  
		adminpanel.asp  
		fileadmin/  
		fileadmin.php  
		fileadmin.asp  
		fileadmin.html  
		administration/  
		administration.php  
		administration.html  
		sysadmin.php  
		sysadmin.html  
		phpmyadmin/  
		myadmin/  
		sysadmin.asp  
		sysadmin/  
		ur-admin.asp  
		ur-admin.php  
		ur-admin.html  
		ur-admin/  
		Server.php  
		Server.html  
		Server.asp  
		Server/  
		wp-admin/  
		administr8.php  
		administr8.html  
		administr8/  
		administr8.asp  
		webadmin/  
		webadmin.php  
		webadmin.asp  
		webadmin.html  
		administratie/  
		admins/  
		admins.php  
		admins.asp  
		admins.html  
		administrivia/  
		Database_Administration/  
		WebAdmin/  
		useradmin/  
		sysadmins/  
		admin1/  
		system-administration/  
		administrators/  
		pgadmin/  
		directadmin/  
		staradmin/  
		ServerAdministrator/  
		SysAdmin/  
		administer/  
		LiveUser_Admin/  
		sys-admin/  
		typo3/  
		panel/  
		cpanel/  
		cPanel/  
		cpanel_file/  
		platz_login/  
		rcLogin/  
		blogindex/  
		formslogin/  
		autologin/  
		support_login/  
		meta_login/  
		manuallogin/  
		simpleLogin/  
		loginflat/  
		utility_login/  
		showlogin/  
		memlogin/  
		members/  
		login-redirect/  
		sub-login/  
		wp-login/  
		login1/  
		dir-login/  
		login_db/  
		xlogin/  
		smblogin/  
		customer_login/  
		UserLogin/  
		login-us/  
		acct_login/  
		admin_area/  
		bigadmin/  
		project-admins/  
		phppgadmin/  
		pureadmin/  
		sql-admin/  
		openvpnadmin/  
		wizmysqladmin/  
		vadmind/  
		ezsqliteadmin/  
		hpwebjetadmin/  
		newsadmin/  
		adminpro/  
		Lotus_Domino_Admin/  
		bbadmin/  
		vmailadmin/  
		ccp14admin/  
		irc-macadmin/  
		banneradmin/  
		sshadmin/  
		phpldapadmin/  
		macadmin/  
		administratoraccounts/  
		admin4_account/  
		admin4_colon/  
		radmind-1/  
		Super-Admin/  
		AdminTools/  
		cmsadmin/  
		phpSQLiteAdmin/  
		server_admin_small/  
		database_administration/  
		system_administration/

## More Content

- https://gist.github.com/jhaddix/2a08178b94e2fb37ca2bb47b25bcaed1 - Github Dorks
