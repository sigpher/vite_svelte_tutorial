<script>
  import HelloWorld from "./lib/HelloWorld.svelte";
  import DynamicAttribute from "./lib/DynamicAttribute.svelte";
  import Assignment from "./lib/Assignment.svelte";
  import UpdatingArraysAndObjects from "./lib/UpdatingArraysAndObjects.svelte";
  import Props from "./lib/Props.svelte";
  import EachBlock from "./lib/EachBlock.svelte";
  import IfBlock from "./lib/IfBlock.svelte";
  import AwaitBlock from "./lib/AwaitBlock.svelte";
  import DomEvent from "./lib/DomEvent.svelte";
  import EventModifiers from "./lib/EventModifiers.svelte";
  import CompoentEvent from "./lib/compoentEvent.svelte";
  import EventForwarding from "./lib/EventForwarding.svelte";
  const handleInfo = (event) => {
    alert(event.detail.content);
  };
  import DomEventForwarding from "./lib/DomEventForwarding.svelte";
  const handleClick = () => {
    alert("Button Clicked");
  };
  import TextInput from "./lib/TextInput.svelte";
  import NumericInput from "./lib/NumericInput.svelte";
  import CheckBoxInput from "./lib/CheckBoxInput.svelte";
  import GroupInput from "./lib/GroupInput.svelte";
  import SelectInput from "./lib/SelectInput.svelte";
  import SelectMultiple from "./lib/SelectMultiple.svelte";
  import Todos from "./lib/Todos.svelte";
  import OnMount from "./lib/OnMount.svelte";
  import Incre from "./lib/store/Incre.svelte";
  import Reset from "./lib/store/Reset.svelte";
  import Decre from "./lib/store/Decre.svelte";
  import { count } from "./lib/store/store";
    import Inner from "./lib/Inner.svelte";
</script>

<!-- 
<HelloWorld />
<DynamicAttribute />
<br />
<Assignment /> -->
<!-- <UpdatingArraysAndObjects></UpdatingArraysAndObjects> -->
<!-- <Props answer="42" /> -->
<!-- <EachBlock></EachBlock> -->
<!-- <IfBlock></IfBlock> -->
<!-- <AwaitBlock /> -->
<!-- <DomEvent></DomEvent> -->
<!-- <EventModifiers></EventModifiers> -->
<!-- <EventForwarding on:info={handleInfo} /> -->
<!-- <DomEventForwarding on:click={handleClick} /> -->
<!-- <TextInput></TextInput> -->
<!-- <NumericInput></NumericInput> -->
<!-- <CheckBoxInput></CheckBoxInput> -->
<!-- <GroupInput /> -->
<!-- <SelectInput></SelectInput> -->
<!-- <OnMount /> -->
<h1>The count is {$count}</h1>
<Incre></Incre>
<Decre></Decre>
<Reset></Reset>