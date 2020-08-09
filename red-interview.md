# The Red Interview Guide

Contents:
 - [Analog and Digital Music Sources](https://profbot.github.io/red-interview#analog-and-digital-music-sources)
 - [Torrenting](https://profbot.github.io/red-interview#torrenting)
 - [Audio Formats](https://profbot.github.io/red-interview#audio-formats)
 - [LAME](https://profbot.github.io/red-interview#lame)
 - [Golden Rules](https://profbot.github.io/red-interview#golden-rules)
 - [CD Ripping and Burning](https://profbot.github.io/red-interview#cd-ripping-and-burning)
 - [Spectral Analysis](https://profbot.github.io/red-interview#spectral-analysis)


### Analog and Digital Music Sources

Music uploaded to RED comes from two main sources: analog media and digital media.
Analog Music Sources

An analog music source must use an analog to digital converter like a sound card to convert physical changes in an analog medium to a digital file that a computer can read. An analog medium is an object that stores music by being physically altered.

For example:

 - A tape recorder changes the magnetization of magnetic tape in a cassette tape to record sound. Plugging a tape deck into a recording device makes a digital copy of the analog cassette tape.
 - A record cutter carves grooves in a vinyl record to make a physical representation of the sound. Ripping vinyl through a preamp and into a sound card makes a digital copy of the analog vinyl.

Analog recordings can be ripped into digital music files, such as FLAC and MP3. Vinyl records are always approved for uploads, but cassettes are only allowed under strict conditions.
Digital Music Sources

A digital music source has already been encoded into a format that a computer can read, so no conversion is necessary. A digital medium is an object that stores music in digital files (a string of binary numbers).

For example:
 - CDs
 - DVDs
 - Super Audio CDs (SACD)
 - WEB downloads (iTunes, Amazon, Artist websites etc.)

Please do not mistake WEB downloads for a non-allowed web rip. Web rips mean a lossy (bad) transcode of an audio stream, such as YouTube, or other streaming services.

Digital music sources can be uploaded to RED after using spectral analysis to check for lossy transcodes.
Analog Music Sources vs. Digital Music Sources

There is still much debate about whether analog and digital sources sound different. Some people prefer the "feel" of vinyl and think that music on vinyl records sounds "warmer" and "fuller". Others think that digital sources provide an unadulterated and pristine listening experience. RED allows both, so you can download and make your own judgment!




### Torrenting

BitTorrent is a system that allows users to share data with each other. Information about the data you want to download is held in a .torrent file, and other people who have added the same .torrent file in their torrent client are called peers. When you download a file, you are leeching from other peers who already have the data. When you finish downloading the file and make yourself available to upload, you are seeding the data to other peers. Although you may have many files seeding, you will not receive upload credit until another peer leeches from you. In other words, you will not gain upload credit for just seeding torrents, though your required ratio will be lower than if you were not seeding torrents. It is possible to seed and leech at the same time because BitTorrent clients download chunks of data, and as soon as your BitTorrent client downloads one chunk of data it may be seeded to other peers. BitTorrent uses a specific protocol based on upload speeds and the number of other peers in order to choose which pieces of the torrent to download from which peer.
Clients

A BitTorrent client is a program that allows you to connect to the BitTorrent system. Think of BitTorrent like the internet and BitTorrent clients as internet browsers. There are multiple different internet browsers with different features, but they connect to the same internet. Click here for the BitTorrent clients that are on the whitelist, or allowed on RED. You will not be able to connect to peers from RED (and thus download data) if your BitTorrent client is not on the whitelist. If there is an "x" behind a decimal, that means that any number can be substituted for the x. For example: uTorrent 2.0.x means that uTorrent 2.0.0, 2.0.1, 2.0.2, 2.0.3, 2.0.4, etc. are all on the whitelist.
Ratio

A ratio is a comparison between your downloaded and uploaded data (this is also known as a fraction). Dividing the amount of data you have uploaded by the amount of data you have downloaded gives you your ratio. A ratio of 1.0 is healthy because it means you have downloaded as much data as you have uploaded. Ratios significantly under 1.0 are unhealthy because it means that you are not contributing as much to the community as you are taking from it. If you have a ratio significantly above 1.0 consider adding bounty's on requests or participating in some of the snatching forum threads. We realize that it may be difficult to maintain a ratio on RED, so we have a ratio system to help out our users. Your required ratio is the ratio you must maintain in order to be able to keep downloading torrents. The required ratio is calculated based on how many torrents you are seeding and how much data you have downloaded.

Notice that your required ratio is much lower if you seed 100% of the torrents you download for at least 72 hours each week. In fact, you would have a required ratio of 0 until you download more than 20 GB if you seed all of your torrents! NOTE: This does not mean you should only seed for 72 hours. It is in your interest, particularly as a new user, to seed for as long as possible. This will help maintain your ratio and help keep content available for everyone.

If you fall below your required ratio, you will be put on ratio watch for two weeks. If you are unable to improve your ratio in this time period, your leeching privileges (ability to download) will be disabled. In order to get your leeching privileges re-enabled, you can fill requests or upload new torrents, as well as continue to seed the torrents you have already downloaded. DO NOT upload torrents that are against the rules, like transcodes, mutt rips, or duplicates. Failing to follow the upload rules, especially when you are in ratio watch, will result in a warning. If you download more than 10 GB while on ratio watch, your leeching privileges will be immediately disabled.
Freeleech and Neutral Leech

Generally the exact amount of data you upload and download is recorded in your ratio. However, there are exceptions to this. Torrents that are marked freeleech or neutral leech do not count towards your ratio in the same way. Neutral leech means none of the data uploaded or downloaded is counted, while freeleech means only your uploaded data is recorded in your ratio. Typically on RED there are no freeleech events where many, or all, torrents are marked as such. Instead we use a system called freeleech tokens, which essentially is a way to mark a torrent as personal freeleech. This means that the data you download does not count towards your ratio, but for everyone else it still does. There are some limitations to these tokens, namely that you can only use them on torrents that are 2GB or less in size, and they are only valid until you have completed your download, or for a total of 96 hours, whichever comes first. You receive tokens during special events or by earning them by helping the site in different ways. Tokens are only valid for a certain period of time.
Port Forwarding

Port forwarding allows computers on the public internet to connect directly to your computer. Most home internet providers use Network Address Translation (NAT) to allow home users to connect as many devices to their router (also known as a modem or wireless unit) as they desire. NAT can also prevent direct connections from the public internet to your computer. Port forwarding tells your router or modem to ensure all requests made on a specific port reach a specific computer inside the NAT. Your BitTorrent client runs on a certain port on your computer (you can assign the port), and by forwarding this port, you make yourself more connectable to other computers. Using port forwarding for connectability increases the chances that your client will upload data to a peer who is leeching.

You can learn more about port forwarding as well as get specific directions on how to set up a port forward on your home router or modem at Port Forward. You can test your port forward by using Can You See Me and putting in your forwarded port number to be tested. You can find which port your BitTorrent client uses under your client's preferences (for uTorrent: Options >; Setup Guide ; for Transmission: Preferences > Network).


#### Partial Seeders

A partial seeder is a peer who has downloaded and is seeding part of a torrent. The peer looks like a leecher; however, they have no intention of downloading the rest of the torrent. Huge torrents like Rosetta Stone Multi-Language MegaPack (38 GB) and a 30 CD Mozart Box Set (50 GB) often have a large number of partial seeders. These torrents should never be downloaded in an attempt to increase ratio.
Marking Torrents As Private

When creating torrents to upload to a private tracker, there is a box to "mark torrent as private". You should always check this box, as it keeps peers who are not members of RED out of the peer list. This is for your security and that of all the site members. Failure to add the private flag to your torrents will result in you having to download the torrent file from the site after uploading.


### Audio Formats

An audio format is a type of computer file that stores music. Music formats are either uncompressed lossless, compressed lossless, or lossy.
Bitrates

A bitrate is the number of bits conveyed or transferred in a unit of time. When talking about music formats, bitrate is used in kilobits per second (kbps). When comparing files with different bitrates (of the same song), the file with the higher bitrate has the higher quality. For example, an MP3 320kbps (CBR) file transfers 320 kilobits per second.
Uncompressed Lossless

Uncompressed lossless formats store all of the original recorded data. Since silence is given the same number of bits per second as sound is, uncompressed lossless files are huge. The main uncompressed lossless format is pulse-code modulation (PCM). For example:

    WAV (PCM) (used on Windows)
    AIFF (PCM) (used on Mac OS)

Compressed Lossless

Compressed lossless formats store all of the original recorded data in less space than uncompressed lossless formats by compressing the data. By giving silence almost no bits per second and compressing sound, a compressed lossless file is usually half as big as the same song stored in an uncompressed lossless file.

Since both uncompressed lossless formats and compressed lossless formats retain all the data from the original recording, they can be transcoded between each other without a loss in quality. For example:

    Free Lossless Audio Codec (FLAC)
    Apple Lossless Audio Codec (ALAC)
    Monkey's Audio (APE)

Lossy

Lossy formats are always compressed. Lossy formats have smaller file sizes than both uncompressed lossless formats and compressed lossless formats because they remove some of the original data. Usually the removed data is in the higher frequencies that humans can't hear, however, there can be obvious audible differences between lossy formats and lossless formats.

Lossy formats CANNOT be transcoded into any other lossy format without losing more quality. It CANNOT be transcoded into lossless either, because it wouldn't be a true lossless file when the source medium is already lossy. Examples of lossy formats include:

    MPEG Layer 3 Audio (MP3)
    Advanced Audio Encoding (AAC)
    Windows Media Audio (WMA)
    Dolby Digital Audio Codec 3 (AC3)
    DTS Coherent Acoustics Codec (DTS)

File Size

Here's an example of how the file size of the same song varies depending on whether the song's format is uncompressed lossless, compressed lossless, or lossy. Let's take the classic pop song, Sk8er Boi by Avril Lavigne. For reference, the song is 3 minutes, 24 seconds long.

    Uncompressed Lossless — WAV (PCM): 34.3 MB
    Compressed Lossless — FLAC: 25.75 MB (25% compressed)
    Lossy — MP3 320 (CBR): 7.78 MB (78% compressed)

Transparency

Transparency is a term used to describe the audible quality of a lossy music file. A lossy file is considered transparent if the average human cannot tell the difference between the lossy file and a lossless file of the same song by just listening to both without knowing which file is which. For most people, MP3 192kbps (CBR) is considered transparent.
Allowed Formats

While there are several types of lossless and lossy music formats, only a few are allowed to be uploaded to RED.

Because lossless formats can be transcoded between each other without a loss in quality, the only allowed lossless format on RED is FLAC. However, you can download the FLAC and convert to ALAC (for iTunes) or whatever lossless or lossy format you prefer.

Only the following lossy music formats are allowed on RED:

    MP3 (the minimum bitrate for MP3 is 192kbps (CBR))
    AAC (can be trumped by any MP3 torrent unless it was bought from the iTunes store and includes iTunes Exclusive tracks)
    AC3 (usually found in DVDs)
    DTS (usually found in DVDs)

MP3 is the most popular lossy format on RED. We allow AAC files bought from the iTunes store because there are often iTunes-specific bonus tracks, and since AAC is lossy it cannot be converted to other formats without a loss in quality. Similarly, AC3 and DTS are music formats often found on DVDs and since they are lossy, they cannot be converted to other formats without a loss in quality.



### LAME

LAME Ain't An MP3 Encoder (LAME) is an encoder that converts and compresses any input audio file and outputs an MP3 file. The resulting MP3 file can have a constant, variable, or average bitrate. RED recommends LAME as an MP3 encoder because it is open source, customizable, and outputs high quality MP3 files.
Constant Bitrate (CBR)

When encoding a constant bitrate (CBR) file, the user (you) chooses a preset bitrate and LAME targets that bitrate throughout the entire file. This means that every second in the file has the same number of bits, no matter how simple or complex the sound is. Every second in a CBR file has the same quality. Because silence is given the same number of bits as more complex sounds, CBR files are larger than VBR and ABR files of the same quality. This also means that CBR files have a predictable file size.
Variable Bitrate (VBR)

When encoding a variable bitrate (VBR) file, the user (you) chooses a preset quality and LAME targets that quality, letting the bitrate vary throughout the entire file. This means that every second of the file has a different number of bits that depends on how complex the sound is at that second. For example, a second of silence would receive much fewer bits than a second of loud, blaring music. Every second can range from 0 to 320kbps (the ceiling for MP3) based on the preset and the audio data being encoded. Since VBR files target a certain quality instead of a certain bitrate, exact VBR file sizes are more unpredictable. The resulting filesize for a VBR encode depends on two factors: the preset selected, and the music itself. The better the preset, the larger the resulting file will be. The more music data necessary to encode, the larger the resulting file will be. When one refers to the 'bitrate' of a VBR file, they are talking about the mean bitrate (in kilobits per second) for the whole song, which is calculated by dividing the filesize by the duration.

LAME has certain VBR presets V0 to V9. V0 is the highest quality VBR preset and V9 is the lowest quality VBR preset. The most popular VBR preset on RED is V0, which usually ends up with a bitrate between 230 and 270 kbps. V2 is the lowest quality LAME VBR preset allowed on RED for music torrents, and generally results in a bitrate between 180 and 210 kbps. At RED, MP3's encoded with the V2 preset are trumpable by those using the V0 preset.
Average Bitrate (ABR)

When encoding an average bitrate (ABR) file, the user (you) chooses a preset bitrate and LAME allows the bitrate to vary throughout the entire file, but the average bitrate of the file will be the bitrate you preset. This means that like CBR, the file size is predictable, and like VBR, the quality and bitrate of the music varies throughout the file depending on how complex the music is each second.

However, ABR is not recommended by RED because it is a mix of both CBR and VBR, and it is thus unable to perform well on either. (Jack of all trades but master of none.)



### Golden Rules

The Golden Rules on RED are as follows:

    Do not create more than one account.
    Users are allowed one account per lifetime. Do not create additional accounts under any circumstance. If your account is disabled, contact staff in #red-disabled on IRC.
    Do not trade, sell, give away, or offer accounts.
    If you no longer wish to use your account, send a Staff PM and request that your account be disabled. Note, we do not delete accounts.
    Do not share accounts.
    Accounts are for personal use only. Granting access to your account in any way (e.g., shared login details, external programs) is prohibited. Invite friends and family if they wish to use the site.
    Do not invite bad users.
    You are responsible for your invitees. You will not be punished if your invitees fail to maintain required share ratios, but invitees who break golden rules or invite rules will place your invite privileges and account at risk.
    Do not trade, sell, publicly give away, or publicly offer invites.
    Only invite people you know and trust. Only Staff and designated recruiters may publicly offer invites on other private trackers. Do not offer invites on public websites or any private sites that exist solely for the purpose of invite giveaways, trading, and/or selling. Do not publicly offer invites on IRC channels or other social chat clients. Offering an invite in a private message to a person you do not know or trust is considered a giveaway and against the rules. Responding to public invite requests is prohibited.
    Do not request invites or accounts.
    Requesting invites to—or accounts on—Redacted or other trackers is prohibited. Invites may be offered, but not requested, in the site's Invites forum (restricted to the Power User class and above). You may request invites by messaging users only when they have offered them in the Invites Forum. Unsolicited invite requests, even by private message, are prohibited.
    Do not engage in ratio manipulation.
    Transferring buffer—or increasing your buffer—through unintended uses of the BitTorrent protocol or site features (e.g., request abuse) constitutes ratio manipulation. When in doubt, send a Staff PM asking for more information.
    Do not report incorrect data to the tracker (i.e., cheating).
    Reporting incorrect data to the tracker constitutes cheating, whether it is accomplished through the use of a modified "cheat client" or through manipulation of an approved client.
    Do not use unapproved clients.
    Your client must be found on the Client Whitelist. You must not use clients that have been modified in any way. Developers interested in testing unstable clients must first receive staff approval.
    Do not modify Redacted .torrent files.
    Embedding non-Redacted announce URLs in Redacted .torrents is prohibited. Doing so causes false data to be reported and will be interpreted as cheating. This applies to standalone .torrent files and .torrent files that have been loaded into a client.
    Do not share .torrent files or your passkey.
    Embedded in each Redacted .torrent file is an announce URL containing your personal passkey. Passkeys enable users to report stats to the tracker.
    Do not blackmail, threaten, or expose fellow users.
    Exposing or threatening to expose private information about users for any reason is prohibited. Private information includes but is not limited to personally identifying information (e.g., names, records, biographical details, photos). Information that hasn't been openly volunteered by a user should not be discussed or shared without permission. This includes private information collected via investigations into openly volunteered information (e.g., Google search results).
    Do not scam or defraud.
    Scams (e.g., phishing) of any kind are prohibited.
    Do not disrespect staff decisions.
    Disagreements must be discussed privately with the deciding moderator. If the moderator has retired or is unavailable, you may send a Staff PM. Do not contact multiple moderators hoping to find one amenable to your cause; however, you may contact a site administrator if you require a second opinion. Options for contacting staff include private message, Staff PM, and #red-disabled on IRC.
    Do not impersonate staff.
    Impersonating staff or official service accounts (e.g., Drone) on-site, off-site, or on IRC is prohibited. This includes impersonating staff of other trackers. Deceptively misrepresenting staff decisions is also prohibited.
    Do not backseat moderate.
    "Backseat moderation" occurs when users police other users. Confronting, provoking, or chastising users suspected of violating rules—or users suspected of submitting reports—is prohibited. Submit a report if you see a rule violation.
    Do not request special events.
    Special events (e.g., freeleech, neutral leech, picks) are launched at the discretion of the staff. They do not adhere to a fixed schedule, and may not be requested by users.
    Do not harvest user-identifying information.
    Using Redacted's services to harvest user-identifying information of any kind (e.g., IP addresses, personal links) through the use of scripts, exploits, or other techniques is prohibited.
    Do not use Redacted's services (including the tracker, website, and IRC network) for commercial gain.
    Commercializing services provided by or code maintained by Redacted (e.g., Gazelle, Ocelot) is prohibited. Commercializing content provided by Redacted users via the aforementioned services (e.g., user torrent data) is prohibited. Referral schemes, financial solicitations, and money offers are also prohibited.
    Do not browse Redacted using public proxies, Tor, or free VPN services.
    Do not browse the site using free proxy or VPN services. Browsing or torrenting through Tor is also forbidden. You may browse the site through paid-for VPN services, private and shared seedboxes, and private servers and proxies. Shared VPNs or VPNs with dynamic IPs need to be approved by staff before use. When in doubt, send a Staff PM seeking approval of your VPN. See our Proxy/VPN Tips and Multiple IPs articles for more information.
    Do not abuse automated site access.
    All automated site access must be done through the API. API use is limited to 5 requests within any 10-second window. Scripts and other automated processes must not scrape the site's HTML pages.
    Do not autosnatch freeleech torrents.
    The automatic snatching of freeleech torrents using any method involving little or no user-input (e.g., API-based scripts, log or site scraping, etc.) is prohibited. See Redacted's Freeleech Autosnatching Policy article for more information.
    Do not seek or exploit live bugs for any reason.
    Seeking or exploiting bugs in the live site (as opposed to a local development environment) is prohibited. If you discover a critical bug or security vulnerability, immediately report it in accordance with Redacted's Responsible Disclosure Policy. Non-critical bugs can be reported in the Bugs Forum.
    Do not publish exploits.
    The publication, organization, dissemination, sharing, technical discussion, or technical facilitation of exploits is prohibited at staff discretion. Exploits are defined as unanticipated or unaccepted uses of internal, external, non-profit, or for-profit services. See Redacted's Exploit Policy article for more information. Exploits are subject to reclassification at any time.

Dupes

A dupe is a torrent that is a duplicate of another torrent that already exists on the site. RED allows many different pressings of the same CD to coexist, as long the the CDs have different content. For example, International Versions (especially Japanese releases) often have bonus tracks that are not present in the original release or the US release. Uploading a release with bonus tracks when the original release has already been uploaded is not considered a dupe because there is different content on both CDs.

    Torrents that have the same bitrates, formats, and comparable or identical sampling rates for the same music release are duplicates. If a torrent is already present on the site in the format and bitrate you wanted to upload, you are not allowed to upload it.
    Scene and non-scene torrents for the same release, in the same bitrate and format, are dupes.
    Rip log information (table of contents, peak levels, and pre-gaps), tracklist, and running order determine distinct editions, not catalog information. Merely having different catalog numbers or CD packaging is not enough to justify a new, distinct edition, though differences in year and label (imprint) do determine distinct releases.
    Torrents that have been inactive (not seeded) for two weeks may be trumped by the identical torrent (reseeded) or by a brand new rip or encode of the album. If you have the original torrent files for the inactive torrent, you should reseed those original files instead of uploading a new torrent.

Trumps

The process of replacing a torrent that does not follow the rules with a torrent that does follow the rules is called trumping. The most common trumps are format trumps, tag trumps, and folder trumps.
Format Trumps

The following chart shows the hierarchy of format trumps.

At the top of each column but the one on the left are formats that can never be trumped. We recommend that you only upload in these formats in order to prevent your torrents from being trumped by other users. If you have the release in lossless/FLAC, we recommend uploading only FLAC, 320 and V0, as these formats will never be trumped by "better" formats. If you only have the release in some other lossy format/bitrate, e.g. MP3 CBR 224 or AAC 256, then feel free to upload it as long as no "better" formats already exist on the site, but understand that your upload may be trumped in the future. Never transcode your lossy files to FLAC, 320 or V0 to prevent them from being format trumped, as the consequences for uploading transcodes are much, much worse.

Lossy Format Trump Rules

    If there is no existing torrent of the album in the allowed format you've chosen, you may upload it in any bitrate that averages at least 192 kbps. (This does not apply to V0 - V2 releases)
    You may always upload MP3 V0 or MP3 320kbps (CBR) as long as another rip with the same bitrate and format doesn't already exist.
    Higher bitrate CBR (Constant Bitrate) and ABR (Average Bitrate) torrents replace lower ones. Once a CBR rip has been uploaded, no CBR rips of that bitrate or lower can be uploaded. In the same manner, once an ABR rip has been uploaded, no ABR rips of that bitrate or lower can be uploaded.
    AAC encodes can be trumped by any allowed MP3 format of the same edition and media. (This does not apply to AAC torrents with files bought from the iTunes Store that contain iTunes Exclusive tracks.)
    Lossy format torrents with .log files, .cue files, .m3u files, and album artwork do not replace equivalent existing torrents.

Lossless Format Trump Rules

    Rips must be taken from commercially pressed or official (artist- or label-approved) CD sources. They may not come from CD-R copies of the same pressed CDs (unless the release was only distributed on CD-R by the artist or label).
    A FLAC torrent without a log (or with a log from a non-EAC or non-XLD ripping tool like dBpoweramp or Rubyripper) may be trumped by a FLAC torrent with a log from an approved ripping tool with any score.
    A FLAC upload with an EAC or XLD log that scores 100% on the log checker replaces one with a lower score. However, no log scoring less than 100% can trump an already existing one that scores under 100% (for example, a rip with a 99% log cannot replace a rip with an 80% log).
    A 100% log rip without a cue sheet can be replaced by a 100% log rip with a noncompliant cue sheet ONLY when the included cue sheet is materially different from "a cue generated from the ripping log." Examples of a material difference include additional or correct indices, properly detected pre-gap lengths, and pre-emphasis flags.

Tag Trumps

Tag trumps happen when the original torrent either doesn't have the required tag fields or the information in one of the tag fields is completely wrong or misspelled. In the case of misspelled words, the spelling must be entirely off in order for the tag trump to be considered (for example, missing articles like "the" or "a", or a couple letters being in the wrong order like "lvoe" instead of "love" is not enough for a tag trump).

    The required tag fields are: title, album, artist, track number.
    Torrent album titles must accurately reflect the actual album titles. Use proper capitalization when naming your albums. Typing the album titles in all lowercase letters or all capital letters is unacceptable and makes the torrent trumpable.
    Newly re-tagged torrents trumping badly tagged torrents must reflect a substantial improvement over the previous tags. Small changes that include replacing ASCII characters with proper foreign language characters with diacritical marks (á, é, í, ó, ú, etc.), fixing slight misspellings, or missing an alternate spelling of an artist (excluding "The" before a band name) are not enough for replacing other torrents.

Folder Trumps

Folder trumps happen when the original torrent's folder is not named like it should be. Folders should at the very least include the album name, but should hopefully also include the year released and music format. Nested folders are also not allowed.

    Music releases must be in a directory that contains the music. This includes single track releases, which must be enclosed in a torrent folder even if there is only one file in the torrent. No music may be compressed in an archive (.rar, .zip, .tar, .iso).
    Name your directories with meaningful titles, such as "Artist - Album (Year) - Format." The minimum acceptable is "Album" although you should include more information.
    Avoid creating unnecessary nested folders (such as an extra folder for the actual album) inside your properly named directory.
    File names must accurately reflect the song titles. You may not have file names like 01track.mp3, 02track.mp3, etc. Torrents containing files that are named with incorrect song titles can be trumped by properly labeled torrents.
    Multiple-disc torrents cannot have tracks with the same numbers in one directory. You may place all the tracks for Disc One in one directory and all the tracks for Disc Two in another directory or prepend your file names with disc numbers, e.g. 1-01 - first track title.mp3, etc. if you put all the files in a single folder.




### CD Ripping and Burning

CD ripping is a way to extract the music files from a CD. CD burning is a way to make a CD from music files.
Log Files

A log file is a text file with the file extension ".log". Like its name suggests, it acts as a log of the entire ripping process and it records any errors that may have occurred. You may not, for any reason, modify a log file. It is strictly against the rules and will result in warnings/loss of upload privilege/account disabling. Click here to see an example of a log file.
Cue Files

A cue file is a text file with the file extension ".cue". Cue files act as a catalog or a table of contents of a CD and allow you to burn a CD identical to an original CD. Click here to see an example of a cue file.
Suggested CD Ripping Programs

RED suggests using Exact Audio Copy (EAC) on Windows or Linux (with Wine), and X Lossless Decoder (XLD) on Mac OS. Both EAC and XLD produce high quality rips with sufficient logs to prove that the files are up to standard.

These programs must be setup according to the guides available on our wiki to ensure quality rips that meet the sites standards.



### Spectral Analysis

Spectral analysis is a visual way to display the data in a music file. Every music note has a specific frequency: lower notes have lower frequencies and higher notes have higher frequencies. All of the frequencies are displayed on a spectral diagram ("spectral" for short), which is a graph of all the frequencies vs. time in a music file. Frequencies are measured in hertz (Hz) and kilohertz (1,000 Hz). Humans have a hearing range from about 20 Hz - 20kHz (20,000 Hz).

Since spectrals show all the data in a file, they are helpful tools to use when you're trying to decide whether or not a song has been transcoded. Every file has a relatively standard frequency cut-off.

Click on any of the spectrals below to view it in a higher resolution.
CD / Lossless

Songs on a retail CD and lossless songs have frequencies that extend all the way to 22 kHz. Since lossless to lossless transcoding preserves all of the data in a music file, the spectral of a lossless song will look the same in FLAC, WAV (PCM), ALAC, etc.

[Spectral (FLAC)]

However, different genres have different-looking spectrals. The example above was a pop song, so most of the frequencies were represented. But look at this classical piano song.

[Spectral (FLAC - Classical)]

It looks much different, right? But it's still a lossless spectral! Notice how "white noise" (the light purple) still extends to 22 kHz, even though those frequencies aren't used.
MP3

Different types of MP3s have different frequency cut-offs. MP3s also tend to have a "shelf" at 16 kHz (you'll see it in the spectrals).

MP3 320kbps (CBR) has a frequency cut-off at 20.5 kHz. [Spectral (MP3 320)]

MP3 256kbps (CBR) has a frequency cut-off at 20 kHz. [Spectral (MP3 256)]

MP3 V0 has a frequency cut-off at 19.5 kHz. [Spectral (MP3 V0)]

MP3 192kbps (CBR) has a frequency cut-off at 19 kHz. [Spectral (MP3 192)]

MP3 V2 has a frequency cut-off at 18.5 kHz. [Spectral (MP3 V2)]

MP3 128kbps (CBR) has a frequency cut-off at 16 kHz. [Spectral (MP3 128)]
Transcodes

How are spectrals helpful when trying to detect transcodes? Say you download a song in FLAC from a blog. The only way to verify that this song is truly a lossless file and not a transcoded file is by looking at its spectral. (Programs like AudioIdentifier are not reliable at detecting transcodes.)

For example, the spectral below is of a FLAC file: the file extension is .flac, it is 21.8 MB, and it sounds okay.

[Spectral (MP3 192 to FLAC)]

But whoa, does that look anything like what a regular FLAC spectral should look like? No! This file was transcoded from MP3 192kbps (CBR) to FLAC. It's a lossy to lossless transcode, which is bad.
Programs

For spectral analysis, we recommend using either Adobe Audition (Windows or Mac OS), Audacity (Windows, Mac OS, Linux), and SoX (Windows, Mac OS, Linux — command line only). All of the spectrals that appear in this guide were viewed in Adobe Audition CS 6.

Although you should use spectral analysis to determine whether a file is a transcode or not, you will need to use another program to first determine what bitrate or encoding preset the file claims to be. For this purpose, we recommend using Audio Identifier or dbPowerAmp on Windows and dnuos or MediaInfo on Mac OS.
