<script lang="ts">
	interface Props {
		work_title: string;
		work_description: string;
        work_link:string;
	};

    const props:Props = $props();
</script>

<div class="work">
	<a href={props.work_link} class="work-title">{props.work_title}</a>
	<p class="work-description">{props.work_description}</p>
</div>

<style>
    .work {

        display: flex;
        flex-direction: column;

        padding: 16px;

        border-color: lightgray;
        border-style: solid;
        border-width: 0px;
        border-top-width: 2px;
        border-bottom-width: 2px;

    }

    .work-title {
        font-size: 24px;
        text-decoration: none;

        padding-left: 16px;
    }

    .work-description {
        color: gray;
        font-size: 16px;

        padding-left: 16px;
    }
</style>
