# DirSpray
DirSpray allows you to take a list of target domains, a list of target files and directories, and then enumerate those without having to throttle your requests. 
<br>
Fingerprints:<br>
Mac: 5769da30441117b6f864aa26a85fd5678f1ee24f<br>
Kali Linux: af7593f25611dfe7872e247817067620a4b7363b<br>
Windows: 2360e9187f033b3b48e8a6011fd739e646372398<br>
<br>
<!-- wp:paragraph -->
<p>Directory spraying is a technique I use to enumerate files and directories while bug bounty hunting. The typical approach is to enumerate all the subdomains you can find and then start working on finding your targets. Part of this process includes discovery lists which could contain thousands of files and directories. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Enumerating a single domain or subdomain for thousands of files or directories at once can overwhelm a site. Organizations typically request that you throttle your request to prevent that from happening. I personally limit my discovery attack within BurpSuite to the parameters:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Maximum concurrent requests: 1</li><li>Delay between requests: 1500</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>The problem with this approach is that it's time consuming to enumerate a large number of files and directories against a target domain and multiple target domains. Directory Spraying allows you to enumerate a larger list of target domains with a smaller list of files and directories.</p>
<!-- /wp:paragraph -->
<br>
Check out my blog post for a full explanation: https://anticrysys.com/directory-spraying-bug-bounties/
