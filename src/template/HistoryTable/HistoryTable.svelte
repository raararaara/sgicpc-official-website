<script>
	export let title, award, thead, tbody;
</script>

<div class="row pad">
	<div class="p25">
		<h2>{title}</h2>
	</div>
	<div class="p75">
		<div class="table_container">
			<table>
				<thead
					><tr>
						{#each thead as data}
							<th>{data}</th>
						{/each}
					</tr></thead
				>
				<tbody>
					{#each tbody as data, idx}
						<tr>
                            <td>{data[0]}<i class={`award ${award[idx]}`} /></td>
                            <td>{data[1]}</td>
                            <td>{data[2]}</td>
                            </tr>
					{/each}
				</tbody>
			</table>
		</div>
	</div>
</div>
