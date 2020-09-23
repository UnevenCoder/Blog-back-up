## 3 reasons you should try Svelte

##### **Svelte** a new contender to the war of **JavaScript frameworks**. It might not be as mature as other frameworks like **React** and **Vue**, but here are three reasons you should try **Svelte**:
- The learning curve is pretty small
- It requires less amount of lines & has easy state management.
- It is not a normal framework.


### 1 . Learning curve is pretty small 

If you know **HTML** ,**CSS** & **Javascript**, learning **Svelte** is going to be a breeze. Like **Vue**, **Svelte** templates are a superset of **HTML**.

A  simple **svelte** example :
![img](https://cdn.discordapp.com/attachments/594557132633014272/758130760699609088/Screenshot_20200923-0355582.jpeg)

In first glance everything looks like **HTML** but it is **Svelte**. The **{}** are usually used to insert **Javascript** in **HTML**.

> **Svelte** is  **HTML ,CSS ,Javascript** with many cool add-ons.

If you know only **HTML ,CSS ,Javascript** than give **Svelte** a try. Later **transitioning** to other frameworks will be easy too.



### 2 . It requires less amount of lines & has easy state management.

Let's take an example of a simple counter with **React** & **Svelte** 

###### React :
```
class Timer extends React.Component {
  constructor(props) {
    super(props);
    this.state = { seconds: 0 };
  }

  tick() {
    this.setState(state => ({
      seconds: state.seconds + 1
    }));
  }
  componentDidMount() {
    this.interval = setInterval(() => this.tick(), 1000);
  }

  componentWillUnmount() {
    clearInterval(this.interval);
  }

  render() {
    return (
      <div>
        Seconds: {this.state.seconds}
      </div>
    );
  }
}

ReactDOM.render(
  <Timer />,
  document.getElementById('timer-example')
);
```

###### Svelte :


```
<script>
  let seconds = 0;
  setInterval(() => seconds += 1, 1000);
</script>

Seconds: {seconds}

```
> React: 33 lines , 
> Svelte: 6 lines

As seen from above :
- **Svelte** does greater things in  few lines of code.
- **Svelte** 's state management is really simple.



### 3 . It isn't a **normal** framework..


Svelte is pretty different from other frameworks. Svelte **compiles** you code into **vanilla javascript**. Thus the build size of Svelte apps is small. Svelte deserves its reputation because of its speed and developer experience.

### Conclusion :

##### Svelte doesn't have a large community like **Vue** nor is being backed  by any major company like **Angular** & **React**. Svelte is growing constantly but it still is pretty young and new in the market. I had suggested using it for personal projects rather than for job hunting etc.

### Resources 

###### Some cool resources you should definitely check out.
 

- [Official Svelte Site](https://svelte.dev/) 
- [Introduction to Svelte](https://youtu.be/qqt6YxAZoOc) 
- [How Svelte is truely Reactive](https://youtu.be/AdNJ3fydeao) 
- [Svelte vs React vs Angular vs Vue](https://youtu.be/DZyWNS4fVE0)


