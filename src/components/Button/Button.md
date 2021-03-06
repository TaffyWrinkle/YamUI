### Notes for use

While buttons can technically be used to navigate a user to another part of the experience, this is not recommended unless that navigation is part of an action or their flow.

Also, use concise, specific, self-explanatory text, usually a single word. They should include a verb. If acting on something, their text should include the noun they're acting on, e.g. *"Create Group"*.

Use `type='submit'` for submitting forms. Doing this will trigger the onClick action when the user presses the enter key within certain form fields.

### Examples

Regular buttons:

```js { "props": { "data-description": "regular" } }
const { ButtonColor, ButtonStatus, ButtonIconPosition, ButtonSize } = require('.');
const Add = require('../Icon/icons/Add').default;
const ChevronRightMed = require('../Icon/icons/ChevronRightMed').default;
const ChevronDownMed = require('../Icon/icons/ChevronDownMed').default;

const sampleText = 'Next';
const sampleUrl = 'https://www.yammer.com';

<table>
  <thead>
    <tr>
      <th style={{ textAlign: 'right' }} />
      <th>Default</th>
      <th>Link</th>
      <th>Disabled</th>
      <th>Loading</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style={{ textAlign: 'right' }}>Primary</td>
      <td>
        <Button
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.DISABLED}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.LOADING}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={Add}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          size={ButtonSize.REGULAR}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.DISABLED}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.LOADING}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.REGULAR}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.DISABLED}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronDownMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.LOADING}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
    </tr>
    <tr>
      <td style={{ textAlign: 'right' }}>Secondary</td>
      <td>
        <Button
          text={sampleText}
        />
      </td>
      <td>
        <Button
          text={sampleText}
          href={sampleUrl}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.DISABLED}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.LOADING}
          text={sampleText}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={Add}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.SECONDARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          size={ButtonSize.REGULAR}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.SECONDARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.DISABLED}
          text={sampleText}
          color={ButtonColor.SECONDARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.LOADING}
          text={sampleText}
          color={ButtonColor.SECONDARY}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.REGULAR}
          text={sampleText}
          color={ButtonColor.SECONDARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.REGULAR}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.SECONDARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.DISABLED}
          text={sampleText}
          color={ButtonColor.SECONDARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronDownMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.LOADING}
          text={sampleText}
          color={ButtonColor.SECONDARY}
        />
      </td>
    </tr>
  </tbody>
</table>
```

Small buttons:

```js { "props": { "data-description": "small" } }
const { ButtonColor, ButtonStatus, ButtonIconPosition, ButtonSize } = require('.');
const Add = require('../Icon/icons/Add').default;
const ChevronRightMed = require('../Icon/icons/ChevronRightMed').default;
const ChevronDownMed = require('../Icon/icons/ChevronDownMed').default;

const sampleText = 'Next';
const sampleUrl = 'https://www.yammer.com';

<table>
  <thead>
    <tr>
      <th style={{ textAlign: 'right' }} />
      <th>Default</th>
      <th>Link</th>
      <th>Disabled</th>
      <th>Loading</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style={{ textAlign: 'right' }}>Primary</td>
      <td>
        <Button
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button size={ButtonSize.SMALL}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.DISABLED}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.LOADING}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={Add}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          size={ButtonSize.SMALL}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button icon={Add}
          status={ButtonStatus.DISABLED}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.LOADING}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.SMALL}
          text={sampleText}
          href={sampleUrl}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.DISABLED}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
      <td>
        <Button
          icon={ChevronDownMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.LOADING}
          size={ButtonSize.SMALL}
          text={sampleText}
          color={ButtonColor.PRIMARY}
        />
      </td>
    </tr>
    <tr>
      <td style={{ textAlign: 'right' }}>Secondary</td>
      <td>
        <Button
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          size={ButtonSize.SMALL}
          text={sampleText}
          href={sampleUrl}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.DISABLED}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          status={ButtonStatus.LOADING}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={Add}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          icon={Add}
          size={ButtonSize.SMALL}
          text={sampleText}
          href={sampleUrl}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.DISABLED}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          icon={Add}
          status={ButtonStatus.LOADING}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
    </tr>
    <tr>
      <td />
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          size={ButtonSize.SMALL}
          text={sampleText}
          href={sampleUrl}
        />
      </td>
      <td>
        <Button
          icon={ChevronRightMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.DISABLED}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
      <td>
        <Button
          icon={ChevronDownMed}
          iconPosition={ButtonIconPosition.RIGHT}
          status={ButtonStatus.LOADING}
          size={ButtonSize.SMALL}
          text={sampleText}
        />
      </td>
    </tr>
  </tbody>
</table>
```

Bistate button - Join/Leave:

```js { "props": { "data-description": "bistate button join-leave" } }
const BistateButton = require('./BistateButton').default;
const CheckMark = require('../Icon/icons/CheckMark').default;
const SignOut = require('../Icon/icons/SignOut').default;

const leaveJoinProps = {
  text: 'Joined',
  icon: CheckMark,
  activeProps: {
    text: 'Leave',
    icon: SignOut,
  },
};

<BistateButton {...leaveJoinProps} />
```

Bistate button - Follow/Unfollow:

```js { "props": { "data-description": "bistate button follow-unfollow" } }
const { ButtonColor } = require('.');
const BistateButton = require('./BistateButton').default;
const CheckMark = require('../Icon/icons/CheckMark').default;
const Remove = require('../Icon/icons/Remove').default;

const followUnfollowProps = {
  text: 'Following',
  icon: CheckMark,
  color: ButtonColor.PRIMARY,
  activeProps: {
    text: 'Unfollow',
    icon: Remove,
    color: ButtonColor.SECONDARY,
  },
};

<BistateButton {...followUnfollowProps} />
```

Link button:

```js { "props": { "data-description": "link" } }
<Button text="I am a link" href="https://www.yammer.com" />
```

Link button with newWindow:

```js { "props": { "data-description": "link with newWindow" } }
<Button text="I am a link that opens in a new window" href="https://www.yammer.com" newWindow={true} />
```

Submit button:

```js { "props": { "data-description": "submit button" } }
<Button text="Submit" type="submit" />
```

Loading button:

```js { "props": { "data-description": "loading" } }
const { ButtonStatus } = require('.');

class LoadingButton extends React.Component {
  constructor(props) {
    super(props);

    this.state = { busy: false };

    this.handleClick = this.handleClick.bind(this);
  }

  render() {
    const { busy } = this.state;

    return (
      <Button
        text="I am really busy"
        status={busy ? ButtonStatus.LOADING : ButtonStatus.ENABLED}
        onClick={this.handleClick}
      />
    );
  }

  handleClick(key) {
    this.setState({ busy: true });
    setTimeout(() => {
      this.setState({ busy: false});
    }, 5000);
  }
}

<LoadingButton />
```

Full width:

```js { "props": { "data-description": "full width" } }
const { ButtonColor } = require('.');
const { FixedGridRow, FixedGridColumn, GutterSize } = require('../FixedGrid');

<div>
  <p>Sometimes a layout can be achieved easier if the button stretches to fill its container's width. Here's an example of <strong>fullWidth</strong> buttons in a grid layout.</p>
  <FixedGridRow bottomSpacing={GutterSize.SMALL}>
    <FixedGridColumn>
      <Button text="Full width" fullWidth={true} />
    </FixedGridColumn>
    <FixedGridColumn fixed={true} width={100}>
      <Button text="Full width" fullWidth={true} />
    </FixedGridColumn>
  </FixedGridRow>
  <Button text="Full width" fullWidth={true} color={ButtonColor.PRIMARY} />
</div>
```

With supported event handlers:

```js { "props": { "data-description": "with event handlers" } }
<Button
  text="Interact with me"
  onClick={action('button clicked')}
  onMouseEnter={action('button mouse enter')}
  onMouseLeave={action('button mouse leave')}
  onFocus={action('button focused')}
  onBlur={action('button blurred')}
/>
```
