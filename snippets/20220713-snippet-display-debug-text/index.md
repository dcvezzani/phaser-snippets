## Snippet Display Debug Text

### Scene

```
    preload(){
        this.load.bitmapFont('courier', 'assets/font/Courier.png', 'assets/font/Courier.fnt')
    }

    create(){
        this.textName = new Phaser.GameObjects.BitmapText(this, 0, 0, 'courier', 'hello', 16, Phaser.GameObjects.BitmapText.ALIGN_LEFT)
    }

    update () {
        if (!!this.textName)
        this.textName.text = [
            `window.outerWidth: ${window.outerWidth}`,
            `window.outerHeight: ${window.outerHeight}`,
            `window.innerWidth: ${window.innerWidth}`,
            `window.innerHeight: ${window.innerHeight}`,
            `game width: ${this.game.config.width}`,
            `game height: ${this.game.config.height}`,
            `window.devicePixelRatio: ${window.devicePixelRatio}`,
        ]        
    }
```

Assets
- [Courier font](/Users/dcvezzani/personal-projects/phaser/cardgame3/assets.zip)

