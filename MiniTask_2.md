1. **TapLock**

**Problem Statement**: 

Unlocking bikes has become extremely difficult, so the ultimate goal of TapLock is to make this process really simple, by providing a locking mount onto the bike, which will open when the correct tapping pattern is applied. This idea allows us to lock and unlock the bike easily. The essence of the product is a microcontroller which can detect and recognise a certain tapping sequence as a password, and can communicate via bluetooth to a phone. However, the exact locking mechanism hasn't really been planned, and the product can be integrated anywhere on the bike to lock.

**Ideation and Planning**:

The current product has the following characteristics which can be improved upon:
- Arduino UNO microcontroller with an accelerometer sensor.
_Advantages_: The Arduino is relatively commonly known and it would be easy to learn how to collect data from the accelerometer sensor. 
_Disadvantages_: It is quite bulky and it might be better to replace it with a smaller microcontroller to keep the product of minimum size.
- Bluetooth connection between phone and microcontroller so that the lock can be controlled from the phone.
_Advantages_: This is a useful mechanism, and it's quite cheap and effective.
_Disadvantages_: Only short-range communication is possible.
- Edge impulse to upload the tap data in order to verify if it matches the password.
_Advantages_: Relatively easy to use for beginners, to create a simple machine learning model, and provides a lot of functionality.
_Disadvantages_: Not a really well-known/common technology, as opposed to creating models directly using libraries on Python.

**Choosing a pipeline**:

Looking at the pros and cons of the technologies used, we can come up with the following improvements:
- First, the Arduino UNO microcontroller needs to be replaced with a relatively less bulky microcontroller, which can be coupled with an accelerometer and a bluetooth module. As the locking mechanism can tend to take up some space, it's better that the microcontroller takes as little space as possible. There are ESP32-based boards in the market that are smaller in size, and have better functionality, so I would suggest using that.
- Regarding the Bluetooth module, for the purpose of this project, it makes sense to only control the lock from short ranges, and hence, there seems no need to upgrade to a wifi module.
- The ML model created on edge impulse probably has no issues, but in case new people are working on the project we can probably recreate the model directly using common Python ML libraries, as they are more widespread and would be a good modification if this project is worked on further in the future.

**Prototyping phase**:

Now, these improvements need to be implemented. The coding needs to be done for the new microcontroller and the prototype can be created again but with these modifications, as I think that will make a big difference to the final product.

2. **Voice-controlled lamp**

**Problem Statement**: 

This project is based on the idea of making a pair of lamps which can be turned on and off using simple voice commands. There are commands that can turn each lamp individually on/off, as well as a command to simultaneously switch both on/off.

**Ideation and Planning**:

The first prototype used an Amazon Echo to collect voice commands and send those signals to the lamp. The following characteristics can be improved upon:
-  Amazon Echo: _Advantages_: It's relatively easy to use and to pair up with your lamps. The voice commands can easily be programmed and be sent to the lamps to change their state. _Disadvantages_: The main disadvantage here is that if we are planning on making a full-fledged product, then we obviously can't be pairing it up with something as expensive as an Amazon Echo, which offers way more features than we require. We can work on a less sophisticated substitute in the second prototype of our product. 

**Choosing a pipeline**:

Now, we need to use a voice recognition module, and work on providing speech recognition functionality to the product. This can then be integrated with the lamps and this can be the basis for the next prototype.

**Prototyping phase**:

Our ideas can be implemented and an appropriate speech recognition module can be created and programmed. Then we'll try to allow it to send signals to the lamp in order to complete our second prototype.

