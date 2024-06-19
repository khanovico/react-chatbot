# Create Chatbot using React 

This project is use react-chatbot-kit for chatbot so you have to install it on your project.


## npm requirements

### `npm react-chatbot-kit`

using this feature you can add your chatbot in your project 
go to
[npm react-chatbot-kit](https://www.npmjs.com/package/react-chatbot-kit)

### `npm bootstrap`

you can use bootstrap in your project for styling your page.
for easy guide go to [npm bootstrap](https://www.npmjs.com/package/bootstrap)

### `npm material-ui`

you can use material ui for easy documentation and effective representation
for easy guide go to [npm material-ui core](https://www.npmjs.com/package/@material-ui/core).

### `npm jquery`

you can use jquery for solve inbuilde jquery
for easy guide go to [npm jquery](https://www.npmjs.com/package/jquery).

## coding section

this section is use for initialize chatbot configurations

<b>Properties:</b>

<b>botName - </b>defines the name of the bot

<b>customStyles -</b> object defining custom styles for different elements.

<b>initialMessages -</b> defines an array of initial messages from the bot. Required property.

<b>state -</b> defines state you want to place into the chatbot component.

<b>customComponents -</b> you can define your own components and swap out the components that come with react-chatbot-kit by replacing them here.

<b>widgets -</b> here you can define a list of widgets that you want to be able to render with a chatbot response.


The message parser controls what happens when the user sends a message.

You have to implement this yourself. The beauty of this is that you can make the message parsing as complex or as simple as you'd like.

The only method that the message parser needs to implement is the "parse" method. This method is called inside the chatbot when it receives a message from the user.


The actionprovider controls what kind of action that the chatbot is going to perform.

The actionprovider is given the createChatBotMessage and createClientMessage functions in the constructor, which you can use to create a new responses.


Widgets are custom components that you can render with chatbot messages.

In order to use widgets, you need to register them in the config. Here you will define the following properties:

widgetName - defines the name of the widget

widgetFunc - define a function that returns the component. The function must take props and spread it into the component.

mapStateToProps - defines which state properties you defined in config should be injected into the widget component.

props - option array of props you want to pass to your component.

When the widget component is rendered it will receive the following props:

actionProvider - the actionprovider class you have defined, so you can trigger other actions from your custom components.

setState - setState function that can manipulate the top level chatbot state.

scrollIntoView - helper function to scroll content into view when doing asynchronous calls, use in combination with useEffect when updating to state to ensure that the chat window is scrolled to bottom.

[state] - any piece of state you defined in the mapStateToProps section of the config.

[props] - any piece of props you defined in the props section of the config.
