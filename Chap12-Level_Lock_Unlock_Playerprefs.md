# Level Lock/Unlock and PlayerPrefs

PlayerPrefs: In order to save the game progress, Unity provides something called “Player Preferences” or ‘PlayerPrefs’ in short. This is a class that stores Player preferences between game sessions. What this means is, say you exit from the game today and re-open it tomorrow, it should be able to save your session and start from where you left off and shouldn’t start from the beginning of the game, what we call as ‘SAVING’ in games.

![save it](https://media.giphy.com/media/t7tP1DI6XfYJFMZZ94/giphy.gif)

PlayerPrefs can store string, float and integer values into the user’s platform registry. The location of saving these values will depend on the type of platform being used as mentioned below.

### **Standalone Player storage location**

On macOS, PlayerPrefs are stored in 

> ~/Library/Preferences/com.ExampleCompanyName.ExampleProductName.plist
> 

Unity uses the same .plist file for projects in the Editor and standalone Players.

On Windows, PlayerPrefs are stored in HKCU\Software\ExampleCompanyName\ExampleProductNamekey.

On Linux, PlayerPrefs are stored in ~/.config/unity3d/ExampleCompanyName/ExampleProductName

On Windows Store Apps, PlayerPrefs are stored in %userprofile%\AppData\Local\Packages\[ProductPackageId]\LocalState\playerprefs.dat

.On Windows Phone 8, Unity stores PlayerPrefs data in the application's local folder. See [Directory.localFolder](https://docs.unity3d.com/ScriptReference/Windows.Directory-localFolder.html)

for more information.

On Android, PlayerPrefs are stored in /data/data/pkg-name/shared_prefs/pkg-name.v2.playerprefs.xml

. Unity stores PlayerPrefs data on the device, in [SharedPreferences](https://codelabs.developers.google.com/codelabs/android-training-shared-preferences/index.html?index=..%2F..android-training#0)

. C#, JavaScript, Android Java and native code can all access the PlayerPrefs data.

On WebGL, Unity stores PlayerPrefs data using the browser's IndexedDB API. For more information, see [IndexedDB](https://developers.google.com/web/ilt/pwa/lab-indexeddb#overview)

**In-Editor Play mode storage location**

On macOS, PlayerPrefs are stored in /Library/Preferences/[bundle identifier].plist

On Windows, PlayerPrefs are stored in HKCU\Software\Unity\UnityEditor\ExampleCompamyName\ExampleProductName key.

Windows 10 uses the application’s PlayerPrefs names. For example, Unity adds a DeckBase string and converts it into DeckBase_h3232628825. The application ignores the extension.  Unity stores PlayerPrefs in a local registry, without encryption. Do not use PlayerPrefs data to store sensitive data.

There are a lot of different data types that can be stored using this class, of course using Get and Set methods they can be fetched and set respectively. The various data types allowed are: 

Float
Int
String

Now for Locking levels, you can create an enum of different statuses as shown below, based on the requirements of your game:

![Status_levels PNG](https://user-images.githubusercontent.com/44625252/152819377-da7eb494-3387-4bbf-b640-6d8871442f47.png)

As shown in the example above, every time a level is completed, you have the status as “Completed”, levels that are unlocked will have the “Unlocked” status, and levels that have not been played yet will be kept as “Locked”. The following shows the buttons for levels, you can design in a similar way: 

![AllLevels PNG](https://user-images.githubusercontent.com/44625252/152819504-e871ef35-4057-4147-acd7-b46a403c9856.png)

Then, for each button, the status can be set based on its state, of course, levels such as the lobby (menu screen) and Level 1 (the very first level) needs to be kept at ‘Unlocked’ status from the beginning so that they can be accessed by the user in the Start itself. The below shows an example of a switch case statement that allows the button click function to work only when the level is in ‘Unlocked’ status: 

![Button_locks PNG](https://user-images.githubusercontent.com/44625252/152819550-bd8d7ea3-07e0-467d-90de-2592c5eac22e.png)

Finally, the PlayerPrefs can be set and fetched as required as shown below:

![Prefs_levelValue PNG](https://user-images.githubusercontent.com/44625252/152819626-36bac7f6-055b-4766-a7bb-29856a7d8308.png)

You can always find the values in your local device in places, for example, the below shows the storage location on a Windows PC (in the registry editor): 

![Reg_ed PNG](https://user-images.githubusercontent.com/44625252/152819685-7342b479-c0b9-49df-a373-7826b1f54b5e.png)

Now, you can come inside the storage location and delete the values manually if you want to not have the saved values for any reason (for example, When the User wants to delete all saves and start a New Game) otherwise, there are 2 other ways to clear all values: 

- Use DeleteAll or DeleteKey functions using the C# script
- Use Clear All Player Prefs option under Edit category:

![ClearAllPrefs](https://user-images.githubusercontent.com/44625252/152819777-a39cdf22-66fb-48b8-8e7b-786f96461e53.png)

---

## Wrapping Up
   
We covered a lot in this one. Feel free to take a breather over here.

Maybe share your progress with the world via LinkedIn & Twitter?

Once you're done posting fill this [form](https://airtable.com/shrXGSkgf5NClpoIU) so that we can also track your progress and give you cool stuff for getting this far!

![feels amazing](https://media.giphy.com/media/iJzUIm93RqJlCfoYn0/giphy.gif)



