# Ion-item-sliding Issue

## Replication Code

```html
<ion-item-sliding>
  <ion-item-options side="start">
    <ion-item-option>Test</ion-item-option>
  </ion-item-options>
  <ion-item>
    <ion-label>Test Slider</ion-label>
    <ion-input></ion-input>
  </ion-item>
</ion-item-sliding>
```

## Replication Steps

1. Click the `ion-label` of the `ion-item`
    - Do NOT let go of the mouse
2. Drag the `ion-item` to the right until the cursor turns into a text-cursor
3. Release the mouse

You will see that the slider slams shut abruptly, and when you open it again the `ion-item-option` is gone.

I believe the cause is that the `ion-item-option` is being pushed out of the view container.
