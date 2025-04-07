<script lang="ts">

    const seoImgHeight = 800;
    const seoImgWidth = 1400;
    const picsumHost = "https://picsum.photos";

    const name = "Wobble Watch";
    const rootUrl = "https://wobblewatch.bybear.dk"

    const title = `${name} | Another round?`;
    const description = `Test your reaction time and scientifically determine if you should get another beer!`;
    const image = $state(`${picsumHost}/id/${146}/${seoImgWidth}/${seoImgHeight}`);
    const type = "website";
    const url = rootUrl;
</script>

<svelte:head>
    <title>{title}</title>
    <link rel="canonical" href={url}>

    <meta name="description" content={description}>
    <meta property="article:publisher" content={rootUrl}>

    <meta property="og:site_name" content={name}>
    <meta property="og:locale" content="da_DK">
    <meta property="og:type" content={type}>
    <meta property="og:url" content={url}>
    <meta property="og:title" content={title}>
    <meta property="og:description" content={description}>
    <meta property="og:url" content={url}>

    <meta property="og:image" content={image}>
    <meta property="og:image:width" content={seoImgWidth.toString()}>
    <meta property="og:image:height" content={seoImgHeight.toString()}>
    <meta property="og:image:type" content="image/jpeg">

    <meta property="twitter:domain" content={rootUrl}>
    <meta property="twitter:url" content={url}>
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content={title}>
    <meta name="twitter:description" content={description}>
    <meta name="twitter:image" content={image}>
</svelte:head>
