<div align="center">

# TraceLabs CTF MVO Award Write-up November, 2025
<img width="150" height="150" alt="TLMVO" src="https://github.com/user-attachments/assets/333a1039-e34a-4ccb-956f-a0006df03cf4" />
</div>

## Team ༼ つ ◕_◕ ༽つ gimmelocation

**OSINTI4L:**
  - [Github](https://github.com/OSINTI4L)

**Delilah - PrincessPi:**
  - [Github](https://github.com/PrincessPi3)
  - Discord: delilahsiabus

**Kara:**
  - [KaraZajac]( https://karazajac.io/)

## Description
This is a write-up of the submission and intelligence gathering workflow used by team ༼ つ ◕_◕ ༽つ gimmelocation in the November, 2025 [TraceLabs](https://tracelabs.org) capture the flag that was ultimately awarded the Most Valuable OSINT (MVO) award.

For privacy reasons to protect the individuals involved redactions have been made.

**MVO Submission:**

<img width="3578" height="1681" alt="MVO-Redacted" src="https://github.com/user-attachments/assets/efb5f241-3036-4e0b-a18d-900312d11d94" />

## Initial Foothold
When the CTF starts each team member typically chooses one missing person (MP) and attempts to gain an initial foothold. A good starting point includes a Google Dork of the MP by name. This will typically return news stories or postings by family members on social media sites related to the disappearance. Multiple images of the MP are typically found when performing this type of search. This allows multiple different angles of photos of the MP to help idenftify and confirm things such as MP social media accounts later on, as well as multiple images to be used with facial recognition tools. Other intel points such as usernames, social accounts, etc. can be found and useful during this time as foothold information to be used as data points to pivot from.

## Locating MP Facebook Account
Delilah began gathering data points on "missing person 1" (MP1). A Facebook (FB) account was found from searching MP1 name on the FB platform. This account could be confirmed owned by the MP via the profile picture consistent with other known photos of the MP. While enumerating the FB account Delilah noticed shared postings from the MP dated less than 24 hours prior to the CTF event. Additionally, multiple data points were found of the MP by Delilah when performing people searches and pivoting from links and profiles linked from her pages.

This yielded:
  - 24 Social media accounts & link directories
  - 14 Usernames
  - 4 Emails
  - 10 Accouts linked to found emails
  - 2 Associated addresses
  - 2 Relatives

Three images specifically stood out as points of focus when enumerating the account:

**Image 1**

The most recent shared post (less than 24 hours prior to the CTF) could be seen in the post history of the MP account. The shared post was originally posted by one of the missing person's friends (MPF) on the MPF Facebook account one day prior to it being shared on the MP profile. The post was an image of the MP inside of what appeared to be a bedroom. The image was analyzed and no identifiers or location relevant data points could be found inside of the image. A thought process here could be, if there are unique identifiers to the structure of the room, locating a residential address (via people search sites, voter registration records, appraisal district lookups) associated with the MP could allow interior images to be found from realtor platforms of the house/apartment by address, thus allowing us to confirm location. Additional data points that could also be useful if found in the image (such as pieces of mail/items with a name listed other than that of the MP) could allow us to attempt to find the residence owner and locate it. Unfortunately, none of the data points were present. Locating the profile was still considered a "win" as it alerted us that the MP was still active and that this specific account was the platform in which they used to post.

**Image 2**

A secondary image was found shared by the MP 5 days prior to the CTF and was originally posted via the MPF FB account 6 days prior to the CTF. The image showed MP and MPF in what appeared to be a photoshoot in an urban area (what appeared to be a car-wash) with a gas station and fast food chain in the immediate vasinity. Geolocation attempts were made to source the location of the images via Google reverse image searching, Google Maps, and AI geo tools: [FindPickLocation](https://findpiclocation.com/). The fruits of our labor were unfortunately sour, so Kara and I began searching for car-washes in known areas of the MP (listed from MP BOLO). This is when Kara's wife overheard the discussion of locating the images that we beleived to be in a specific city/state (via the voice chat we use for team communication). Being familiar with the area she was able to use known knowledge of the city's demographics and apply them to what was seen inside of the image, deriving the location.

The following data points stood out as demographic identifiers:
  - Language of text used on a billboard seen inside of the image
  - The lack of graffiti indicated that it was not in traditional gang neighborhoods
  - The car-wash tiles and paint were not sun bleached which indicates that it was not in an area where taller buildings were present to shade them
  - The car-wash was self-service which was typically not found in the downtown areas

These data points allowed a narrowing of the car-wash search areas and ultimately yielded us an address to the car-wash identified im the image. Google Maps and Google Street View were then utilized to attempt to locate and confirm the *exact* location that the image was taken. Specific identifers seen in the image such as the cleaning station, satellite dish/window positions, and matching fance-line (seen in above submission image), allowed us to confirm the location of the image down to the exact position where the image was taken.

**Image 3**

The last image analyzed was a video shared by the MP 12 days prior to the CTF and originally posted by the MPF earlier in the year post dissapearance. The video showed the MP standing infront of a lighting structure looking around and putting on a hat. An approximate one second frame can be seen in the video while the camera angle moves of a building in the background with a "casino" sign atop. This allowed us to locate the building via Google searches, Google Maps, and Google Street View. Utilizing Google Street View we then attempted to locate the lighting structure seen in close proximity to the "casino" building. The lighting structure was ultimately found and confirmed by comparing various data points such as a matching padlock and storage area, matching lighting, and a Chevron gas station sign that could be seen to the left of the lighting strucutre that was present in the video frame (see MVO submission). This was the exact location that the video was recorded.

**Pulling It All Together**

As we decided that the aforementioned data points were the *most* relevant to the investigation, we began documenting. A flow chart was made (draw.io) with all relevant intel points gathered. This allowed us to provide a single document showing the workflow and comparison of geolocation data showing how the information was sourced and how we confirmed the intel was valid. Information without context is not intelligence, as such, we have found that the proper documentation of intel points is *just as important* as the intel points themselves. This chart allowed us to ultimately display that and thus awarded Most Valuable OSINT.

✌️
