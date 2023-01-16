<script>
    let m = { x: 0, y: 0 };
</script>

<div on:mousemove={(e) => (m = { x: e.clientX, y: e.clientY })}>
    The position of m is {m.x} x {m.y}
</div>
