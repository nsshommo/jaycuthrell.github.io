---
layout: post
title: "Converged Thoughts: Issue 5"
date: 2016-12-30 10:24
redirect_from:
  - /issues/converged-thoughts-5-oops-41066
tags:
 - digest
---

<!DOCTYPE html>
<html>
<head>
<meta charset='utf-8'>
<meta content='IE=edge,chrome=1' http-equiv='X-UA-Compatible'>
<title dir='ltr'>Revue - Get your thoughts into people's inboxes</title>
<meta content='width=device-width, initial-scale=1.0' name='viewport'>
<meta content='We believe everybody should send a newsletter. We are here to make it extremely simple to send yours today and start a conversation with your followers.' name='description'>
<meta content='newsletter, email, digest, curation' name='keywords'>
<!--[if lt IE 9]>
<script src="//d3jbm9h03wxzi9.cloudfront.net/assets/html5shiv-d3d35aa8c5c7074d41080b04f1324ad142a05add2f6e1e2ac7028b1eb3bece66.js"></script>
<![endif]-->
<link rel="stylesheet" media="all" href="//d3jbm9h03wxzi9.cloudfront.net/assets/application-5382751a4a02b2ae0beab6e881b3b266787f8ad475658281d558ad532e78c053.css" />
<script src="//d3jbm9h03wxzi9.cloudfront.net/assets/application-68149966cfd9f7c56685ab6ec31040c0ac2420a14a1582b46e7bdeb678907958.js"></script>
<script>
  I18n.defaultLocale = "en";
  I18n.locale = "en";
</script>
<link href='//d3jbm9h03wxzi9.cloudfront.net/assets/favicon-84fc7f228d52c2410eb7aa839e279caeaa491588c7c75229ed33e1c7f69fe75d.ico' rel='icon' size='16x16'>
<link href='//d3jbm9h03wxzi9.cloudfront.net/assets/favicon-84fc7f228d52c2410eb7aa839e279caeaa491588c7c75229ed33e1c7f69fe75d.ico' rel='icon' size='32x32'>
<link color='#E15718' href='//d3jbm9h03wxzi9.cloudfront.net/assets/icon-3c1cfdd15627dced20a77f68d16ee564dc20eed0e312dd9c1bf8051c15691617.svg' rel='mask-icon'>
<meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="8CRJxSUHA/tUvF//zCXNOmAALLqXhsX7yp/UfnIxVW0YoEsmKtsQa0lwYsl4kGZw/9ifn0TmcIbl+tZ6UyA1RQ==" />

<link rel="stylesheet" media="screen" href="https://fonts.googleapis.com/css?family=Bevan" />
<script type="text/javascript">
  function getQueryParam(url, param) {
    // Expects a raw URL
    param = param.replace(/[\[]/, "\\\[").replace(/[\]]/, "\\\]");
    var regexS = "[\\?&]" + param + "=([^&#]*)",
    regex = new RegExp( regexS ),
    results = regex.exec(url);
    if (results === null || (results && typeof(results[1]) !== 'string' && results[1].length)) {
      return '';
    } else {
      return decodeURIComponent(results[1]).replace(/\+/g, ' ');
    }
  };

  function geUtmParams() {
    var campaign_keywords = 'utm_source utm_medium utm_campaign utm_content utm_term'.split(' ')
    , kw = ''
    , params = {}
    , first_params = {}
    , result = {};

    var index;
    for (index = 0; index < campaign_keywords.length; ++index) {
      kw = getQueryParam(document.URL, campaign_keywords[index]);
      if (kw.length) {
        params[campaign_keywords[index] + ' [last touch]'] = kw;
      }
    }
    for (index = 0; index < campaign_keywords.length; ++index) {
      kw = getQueryParam(document.URL, campaign_keywords[index]);
      if (kw.length) {
        first_params[campaign_keywords[index]] = kw;
      }
    };

    result.first_params = first_params;
    result.params = params;

    return result;
  }

  function extractReferrer(referrer) {
    campaign = geUtmParams().first_params["utm_campaign"];
    ref = getQueryParam(document.URL, 'ref');

    if(!!campaign) {
      return campaign;
    } else if (referrer.search('https?://(.*)google.([^/?]*)') === 0) {
      return 'Google';
    } else if (referrer.search('https?://(.*)bing.([^/?]*)') === 0) {
      return 'Bing';
    } else if (referrer.search('https?://(.*)yahoo.([^/?]*)') === 0) {
      return 'Yahoo';
    } else if (referrer.search('https?://(.*)facebook.([^/?]*)') === 0) {
      return 'Facebook';
    } else if (referrer.search('https?://(.*)twitter.([^/?]*)') === 0 || referrer.search('https?://(.*)t.co/') === 0) {
      return 'Twitter';
    } else if (referrer.search('https?://(.*)linkedin.([^/?]*)') === 0) {
      return 'LinkedIn'
    } else if (referrer == '$direct' || (!referrer || /^\s*$/.test(referrer))) {
      return '$direct';
    } else if (referrer.search('https?://(.*)getrevue.co') == 0) {
      if(/\/app\//.test(referrer)) {
        return 'Revue App';
      } else if (/\/profile\/(.*?)\/issue/.test(referrer)) {
        return 'Revue Profile Issue'
      } else if (/\/profile\//.test(referrer)) {
        return 'Revue Profile'
      } else {
        return 'Revue Page'
      }
    } else if (referrer.search('https?://(.*)rev.vu([^/?]*)') === 0) {
      return 'Revue Item';
    } else if (!!ref) {
      return ref;
    } else {
      tld = new RegExp('\.(asn\.au|com\.au|net\.au|id\.au|org\.au|edu\.au|gov\.au|csiro\.au|act\.au|nsw\.au|nt\.au|qld\.au|sa\.au|tas\.au|vic\.au|wa\.au|co\.at|or\.at|priv\.at|ac\.at|avocat\.fr|aeroport\.fr|veterinaire\.fr|co\.hu|film\.hu|lakas\.hu|ingatlan\.hu|sport\.hu|hotel\.hu|ac\.il|co\.il|org\.il|net\.il|k12\.il|gov\.il|muni\.il|idf\.il|ac\.za|gov\.za|law\.za|mil\.za|nom\.za|school\.za|net\.za|co\.uk|org\.uk|me\.uk|ltd\.uk|plc\.uk|net\.uk|sch\.uk|ac\.uk|gov\.uk|mod\.uk|nhs\.uk|police\.uk)')
      a = document.createElement('a');
      a.href = referrer;
      ref = a.hostname;
      if(tld.test(ref)) {
        return ref.replace(tld, '').split('.').pop()
      } else {
        return ref.split('.').reverse()[1];
      }
    }
  };

  function getReferrer() {
    ref = document.referrer;
    return extractReferrer(ref);
  }
  
  function setSource() {
    try {
      initial_ref = mixpanel.get_property('$initial_referrer');
      mixpanel.register_once({"Source": extractReferrer(initial_ref)});
      mixpanel.people.set_once({"Source": extractReferrer(initial_ref)});
      mixpanel.people.set_once({"$created": new Date().toISOString()});
    } catch(e) {}
  };
</script>
<script type="text/javascript">(function(e,b){if(!b.__SV){var a,f,i,g;window.mixpanel=b;b._i=[];b.init=function(a,e,d){function f(b,h){var a=h.split(".");2==a.length&&(b=b[a[0]],h=a[1]);b[h]=function(){b.push([h].concat(Array.prototype.slice.call(arguments,0)))}}var c=b;"undefined"!==typeof d?c=b[d]=[]:d="mixpanel";c.people=c.people||[];c.toString=function(b){var a="mixpanel";"mixpanel"!==d&&(a+="."+d);b||(a+=" (stub)");return a};c.people.toString=function(){return c.toString(1)+".people (stub)"};i="disable time_event track track_pageview track_links track_forms register register_once alias unregister identify name_tag set_config people.set people.set_once people.increment people.append people.union people.track_charge people.clear_charges people.delete_user".split(" ");
for(g=0;g<i.length;g++)f(c,i[g]);b._i.push([a,e,d])};b.__SV=1.2;a=e.createElement("script");a.type="text/javascript";a.async=!0;a.src="undefined"!==typeof MIXPANEL_CUSTOM_LIB_URL?MIXPANEL_CUSTOM_LIB_URL:"file:"===e.location.protocol&&"//cdn.mxpnl.com/libs/mixpanel-2-latest.min.js".match(/^\/\//)?"https://cdn.mxpnl.com/libs/mixpanel-2-latest.min.js":"//cdn.mxpnl.com/libs/mixpanel-2-latest.min.js";f=e.getElementsByTagName("script")[0];f.parentNode.insertBefore(a,f)}})(document,window.mixpanel||[]);
mixpanel.init("2087bc32dd14049d6de8a339112517d9", {loaded: setSource});</script>

<script type="text/javascript">
  var utm = geUtmParams();
  mixpanel.register(utm.params);
  mixpanel.people.set(utm.params);
  mixpanel.people.set_once(utm.first_params);
</script>
</head>
<body class='profiles archive' data-page='ProfilesArchive'>
<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-58968534-1', 'auto');
  ga('send', 'pageview');
</script>
<!doctype html>
<html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
<head>
  <title></title>
  <!--[if !mso]><!-- -->
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <!--<![endif]-->
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<style type="text/css">
  #outlook a { padding: 0; }
  .ReadMsgBody { width: 100%; }
  .ExternalClass { width: 100%; }
  .ExternalClass * { line-height:100%; }
  body { margin: 0; padding: 0; -webkit-text-size-adjust: 100%; -ms-text-size-adjust: 100%;-webkit-font-smoothing: antialiased; -moz-osx-font-smoothing: grayscale;}
  table, td { border-collapse:collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; }
  img { border: 0; height: auto; line-height: 100%; outline: none; text-decoration: none; -ms-interpolation-mode: bicubic; }
  p { display: block; padding: 0; margin: 0; margin-bottom: 0; }
  .revue-p + .revue-p, .revue-p + .revue-blockquote {margin-top: 14px !important;}
</style>
<!--[if !mso]><!-->
<style type="text/css">
  @media only screen and (max-width:480px) {
    @-ms-viewport { width:320px; }
    @viewport { width:320px; }
  }
</style>
<!--<![endif]-->
<!--[if mso]>
<xml>
  <o:OfficeDocumentSettings>
    <o:AllowPNG/>
    <o:PixelsPerInch>96</o:PixelsPerInch>
  </o:OfficeDocumentSettings>
</xml>
<![endif]-->
<!--[if lte mso 11]>
<style type="text/css">
  .outlook-group-fix {
    width:100% !important;
  }
</style>
<![endif]-->
<style type="text/css">
  @media only screen and (min-width:480px) {
    .mj-column-per-100, * [aria-labelledby="mj-column-per-100"] { width:100%!important; }
.mj-column-per-100, * [aria-labelledby="mj-column-per-100"] { width:100%!important; }
.mj-column-per-25, * [aria-labelledby="mj-column-per-25"] { width:25.9259259259%!important; }
.mj-column-per-74, * [aria-labelledby="mj-column-per-74"] { width:74.0740740741%!important; }
  }

  @media only screen and (max-width:480px) {
    .indented {padding-left: 20px !important; padding-right: 20px !important;}
    .link-image {width: 112px !important;}
  }
</style>
</head>
<body>
  <div>
      <div style="display:none;font-size:1px;color:#FFF;line-height:1px;max-height:0px;max-width:0px;opacity:0;overflow:hidden;">Two digests in one day? Well... I&#39;m still new to Revue and missed my edits on the last digest. Thanks</div>

      
    

      <!--[if mso | IE]>
  <table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
    <tr>
      <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
  <![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-top:48px;"><!--[if mso | IE]>
  <table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
  <![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="center"><table role="presentation" cellpadding="0" cellspacing="0" style="border-collapse:collapse;border-spacing:0px;" align="center" border="0"><tbody><tr><td style="width:600px;"><img alt="Jay Cuthrell" title="" height="auto" src="https://s3.amazonaws.com/revue/profile_covers/images/000/000/668/cover/convergedthoughts.png?1483225375" style="border:none;border-radius:0;display:block;outline:none;text-decoration:none;width:100%;height:auto;" width="600"></td></tr></tbody></table></td></tr></tbody></table></div><!--[if mso | IE]>
  </td></tr></table>
  <![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
  </td></tr></table>
  <![endif]-->


    <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-left:30px;padding-right:30px;padding-top:48px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-bottom:10px;" align="left"><div style="cursor:auto;color:#223043;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:30px;font-weight:700;line-height:36px;text-align:left;">
      Converged Thoughts #5 (oops!)
    </div></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:16px;line-height:20px;text-align:left;font-weight:500;color: #9932CC;">
      By <a style="color: #9932CC" href="http://digest.jaycuthrell.com/?utm_campaign=Issue&amp;utm_content=profileimage&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">Jay Cuthrell</a>&nbsp;&bull;&nbsp;Issue #5
    </div></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-top:28px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;"><div style="margin: 0;" class="revue-p">Two digests in one day? Well… I’m still new to Revue and <a href="http://digest.jaycuthrell.com/issues/converged-thoughts-4-41025" style="color: #3498DB" target="_blank">missed my edits on the last digest</a>. Thanks for sticking around and Happy New Year!</div>

    </div></td></tr>
      <tr><td style="word-break:break-word;font-size:0px;padding:60px 0px;"><p style="font-size:1px;margin:0px auto;border-top:2px solid #E7E9EB;width:30px;"></p><!--[if mso | IE]><table role="presentation" align="center" border="0" cellpadding="0" cellspacing="0" style="font-size:1px;margin:0px auto;border-top:2px solid #E7E9EB;width:30px;" width="30"><tr><td style="height:0;line-height:0;"> </td></tr></table><![endif]--></td></tr>
  </tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->

    
      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-bottom:24px;" align="left"><div style="cursor:auto;color:#E15718;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:24px;font-weight:700;line-height:32px;text-align:left;color: #9932CC;">
      2007: Life in the &quot;Foist&quot; Lane (continued)
    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;">
      <div style="margin: 0;" class="revue-p">As I was saying… the way we consume music is changing due to convergence BUT I left a VERY important device! As we entered 2007, there was a steady rise of embedded computing that has slowly taken away the qwerty keyboards that are visually associated with computers. One example that got a lot of attention a decade ago was the humble but ill fated <a href="https://en.wikipedia.org/wiki/Chumby" style="color: #3498DB" target="_blank">Chumby</a>! A chumby could stream all your favorite Internet music streaming stations.</div><div style="margin: 0;" class="revue-p">The time of the internet connected computing capable <i style="">appliance</i> had arrived. Thanks Chumby!</div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="https://en.wikipedia.org/wiki/Chumby?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/237/thumb/384px-Chumby_rear_close-up.jpg?1483303745" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://en.wikipedia.org/wiki/Chumby?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Chumby - Wikipedia</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Little. Alarm clock sized. Always connected.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/wEOeM?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">en.wikipedia.org</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/wEOeM?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;">
      <div style="margin: 0;" class="revue-p">I also missed mentioning the rise of a new category of converged connectivity in 2007 that combined mobile access to IP networks with a localized WiFi service. These devices were accurately dubbed <a href="http://www.waav.com/?q=content/press-release-2-13-07" style="color: #3498DB" target="_blank">hotspots</a>. These hotspots found their way into offices, homes, and even cars… Hmmm… cars….<br style="">
</div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="https://en.wikipedia.org/wiki/Mobile_broadband_modem?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue#Integrated_router">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/328/thumb/220px-HSDPA_cellular_router.jpg?1483306696" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://en.wikipedia.org/wiki/Mobile_broadband_modem?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue#Integrated_router">Mobile broadband modem - Wikipedia</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">A mobile broadband modem, also known as a connect card or data card, is a type of modem that allows a laptop, a personal computer or a router to receive Internet access via a mobile broadband connection instead of using telephone or cable television lines. A mobile Internet user can connect using a wireless modem to a wireless Internet Service Provider (ISP) to get Internet access.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/DOm6k?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">en.wikipedia.org</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/DOm6k?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-bottom:24px;" align="left"><div style="cursor:auto;color:#E15718;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:24px;font-weight:700;line-height:32px;text-align:left;color: #9932CC;">
      2017: Life in the &quot;Feisty&quot; Lane (continued)
    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;">
      <div style="margin: 0;" class="revue-p">Again… As I was saying… consuming music over the past 20 years is changing due to convergence BUT I left off at ANOTHER very important kind of device! </div><div style="margin: 0;" class="revue-p">To recap:</div><div style="margin: 0; display: block; Margin: 0; Margin-bottom: 14px; padding: 0 20px; border-color: #E0E4E8; border-left: 2px solid #E0E4E8; color: #7A889A; line-height: inherit;" class="revue-blockquote">As we enter 2017, it’s amazing to think about what you can do on a smart phone. Things are a bit feisty now and the number of choices are only just beginning.<br style="">Convergence has been embraced in our devices, in how we think about the back end systems that power the experiences made possible by and on those devices, and in our collective consumer expectations. It all should “just work” in ways that would have seemed like actual science fiction in 1997.<br style="">Right now, you have far less parts but oddly enough… quite a few choices to make:<br style=""><ul style="">
<li style="">Device<br style="">
</li>
<li style="">iPhone<br style="">
</li>
<li style="">Android device<br style="">
</li>
<li style="">A netbook, laptop, or yes… a desktop</li>
</ul>
</div><span style=""><div style=""><span style=""><br style=""></span></div></span><div style="margin: 0;" class="revue-p"><span style="">Now, we already know I missed both <i style="">appliances</i> and <i style="">hotspots</i>… </span></div><div style="margin: 0;" class="revue-p"><span style="">What I also missed was the expansion of the connected device <i style="">appliance</i> to come with… wheels.</span></div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=Ldyx3KHOFXw">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/248/thumb/hqdefault.jpg?1483304511" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=Ldyx3KHOFXw">Gary Numan - Cars - YouTube</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Suggested soundtrack for this digest…</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/PQZdW?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.youtube.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/PQZdW?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;">
      <div style="margin: 0;" class="revue-p">Think about cars for a moment. Go ahead. Hit play on the link.</div><div style="margin: 0;" class="revue-p">Clearly, cars existed in 1997. Cars also existed in 2007. Listening to music in a car is just part of growing up in a world where cars existed.</div><div style="margin: 0;" class="revue-p">You could even make the case that one of the major expansions of applied technology in 2007 was the creation of an entire category of geolocation services that went from fleet management vehicles (vans, delivery trucks, etc.) into our pockets as Apps such as Dodgeball and Foursquare.</div><div style="margin: 0;" class="revue-p">On the flip side of connectivity and all things mobile, 2007 also saw the rise of a category of networking devices called hotspots but also better known as mobile access routers by networking folks (which, again, I missed in my prior digest).</div><div style="margin: 0;" class="revue-p">What this means for cars in 2017 is even more convergence. Cars are often the subject of Internet of Things (IoT) discussions because they are accessible examples that many people use.</div><div style="margin: 0;" class="revue-p">You’ve probably heard that a modern car could send as much as multiple terabytes of data ever day to the cloud. You’ve probably also heard that we were promised jet packs. <span style="">Somewhere in the middle is probably accurate though. </span>
</div><div style="margin: 0;" class="revue-p"><span style="">But we’re getting off course…</span></div><div style="margin: 0;" class="revue-p"><span style=""><b style="">Music!</b></span></div><div style="margin: 0;" class="revue-p">Cars will produce a lot more information but let’s take this back to music. Appliances are not laptops or desktops but again let’s take this back to music. We want to listen to music.</div><div style="margin: 0;" class="revue-p">Well, in 2017… we have a lot of options… and things are feisty right now.</div><div style="margin: 0;" class="revue-p">Now you can use various handheld tablets, netbooks, laptops, computers, and even more thanks to music listening cabable appliance form factors.</div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="https://madeby.google.com/home/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="left" style="padding-right: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/333/thumb/home_banner.jpg?1483306856" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://madeby.google.com/home/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Google Home – Made by Google</a></div>
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Hands-free help from the Google Assistant. Enjoy music, get answers, manage your everyday tasks, and control smart devices.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/lyENV?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">madeby.google.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/lyENV?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="https://www.amazon.com/Amazon-Echo-Alexa-Family/b/ref=s9_acss_bw_cg_ODSAuCC_md1_w?node=9818047011&amp;pf_rd_i=9818047011&amp;pf_rd_m=ATVPDKIKX0DER&amp;pf_rd_p=3cb424d0-a34e-448f-9c50-cadfcf8d9fe7&amp;pf_rd_r=F78A1C6GBSR4ZDFATNKC&amp;pf_rd_s=merchandised-search-3&amp;pf_rd_t=101&amp;utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue#compare">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/334/thumb/alexa-cp-smarthome._V527808781_.jpg?1483306909" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://www.amazon.com/Amazon-Echo-Alexa-Family/b/ref=s9_acss_bw_cg_ODSAuCC_md1_w?node=9818047011&amp;pf_rd_i=9818047011&amp;pf_rd_m=ATVPDKIKX0DER&amp;pf_rd_p=3cb424d0-a34e-448f-9c50-cadfcf8d9fe7&amp;pf_rd_r=F78A1C6GBSR4ZDFATNKC&amp;pf_rd_s=merchandised-search-3&amp;pf_rd_t=101&amp;utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue#compare">Echo &amp; Alexa - Amazon Devices - Amazon Official Site</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Echo and other Alexa devices let you instantly connect to Alexa to play music, control your smart home, get information, news, weather, and more using just your voice.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/Z3Zbl?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.amazon.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/Z3Zbl?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;">
      <div style="margin: 0;" class="revue-p">And of course, there are cars. New cars have new options for listening to music. It’s not just about radio, CD, XM satellite or even the Bluetooth or AUX port connected device you already would have in your pocket… it’s connected music over the Internet.</div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="http://zubie.com/in-car-wifi-hotspot/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/338/thumb/GettyImages-483595983_low.jpg?1483307309" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="http://zubie.com/in-car-wifi-hotspot/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Zubie: In Car WiFi Hotspot powered by Verizon 4G LTE Network.</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">*Requires activation on a valid Verizon data plan at point of sale or online.  Not available on unlimited data plans.  $10 monthly fee includes Zubie connected car service and Verizon access charge.  Does not include Verizon data or activation fees, which vary based on your shared data plan.  For more details on how to activate, click here.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/1xARV?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">zubie.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/1xARV?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100" style="vertical-align:top;display:inline-block;font-size:0px;line-height:0px;text-align:left;width:100%;"><!--[if mso | IE]>
<table  role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:13px;line-height:22px;text-align:left;">
          <a target="_blank" style="text-decoration: none;" href="http://www.chevrolet.com/4g-lte-in-car-wifi.html?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/663/337/thumb/2016-bb-chevrolet-4G-LTE-masthead-1480x551.jpg?1483307185" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="http://www.chevrolet.com/4g-lte-in-car-wifi.html?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">4G LTE In-Car Wi-Fi: Features &amp; Information | Chevrolet</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Discover how Chevy’s 4G LTE in-car Wi-Fi is the most reliable way to stay connected while on the go.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/wEOkX?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.chevrolet.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/wEOkX?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
        </div>
      </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


      <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;padding-left:30px;padding-right:30px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;">
      <div style="margin: 0;" class="revue-p">The next question as we enter 2017 is to answer isn’t when will saying “Alexa play music” or “Ok Google play music” or “Siri play music” be possible in your next car… but when will it “just work” because of convergence.</div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->

        <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;"><div style="font-size:1px;line-height:22px;"> </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->


    <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><table role="presentation" cellpadding="0" cellspacing="0" style="background:#FAFAFB;font-size:0px;width:100%;" border="0"><tbody><tr><td><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:64px;padding-left:30px;padding-right:30px;padding-top:64px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-bottom:16px;" align="center"><table role="presentation" cellpadding="0" cellspacing="0" style="border-collapse:collapse;border-spacing:0px;" align="center" border="0"><tbody><tr><td style="width:84px;">
    <a style="text-decoration: none;" target="_blank" href="http://digest.jaycuthrell.com/?utm_campaign=Issue&amp;utm_content=profileimage&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">
      <img alt="Jay Cuthrell" title="Jay Cuthrell" height="84px" width="84" style="border:none;border-radius:0;display:block;outline:none;text-decoration:none;width:100%;height:84px;" src="https://s3.amazonaws.com/revue/profiles/images/000/021/457/small/Jpc0KbFA.png?1482865303" />
</a>  </td></tr></tbody></table></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-bottom:8px;" align="center"><div style="cursor:auto;color:#223043;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:20px;font-weight:700;line-height:24px;text-align:center;">
      By <a style="color: #223043;" href="http://digest.jaycuthrell.com/?utm_campaign=Issue&amp;utm_content=profilename&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">Jay Cuthrell</a>
    </div></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="center"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:16px;line-height:28px;text-align:center;">
        This digest revisits & expands items I've shared that don't fit into 140 characters. Enjoy.
    </div></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-top:32px;" align="center"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:16px;line-height:20px;text-align:center;">
            <a target="_blank" style="color: #1DA1F2; text-decoration: none;" href="https://www.twitter.com/share?url=http://digest.jaycuthrell.com/archive/41066&amp;via=revue&amp;text=Converged%20Thoughts%20%235%20%28oops%21%29%20by%20%40JayCuthrell&amp;related=revue">
              <img alt="" width="24" height="20" style="border:none;border-radius:0;outline:none;text-decoration:none;vertical-align:middle;padding-right:3px;" src="//d3jbm9h03wxzi9.cloudfront.net/assets/email/share_twitter_2-c23bb19c3c2dbb4d69a4a5d6630babeab20cda45cf6876450e97cd68b50d2e60.png" />
              <strong style="color: #1DA1F2;vertical-align:middle;">Tweet</strong>
</a>               
            <a target="_blank" style="color: #3B5998; text-decoration: none;" href="http://www.facebook.com/sharer/sharer.php?u=http://digest.jaycuthrell.com/archive/41066">
              <img alt="" width="20" height="20" style="border:none;border-radius:0;outline:none;text-decoration:none;vertical-align:middle;padding-right:3px;" src="//d3jbm9h03wxzi9.cloudfront.net/assets/email/share_facebook_2-ed8f4e8cbe9cd64529b8d3f1651b4dca46f46d0d0e7d43120462b92f504e8097.png" />
              <strong style="color: #3B5998;vertical-align:middle;">Share</strong></a>
</a>          </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div></td></tr></tbody></table><!--[if mso | IE]>
</td></tr></table>
<![endif]-->

    <!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width:600px;">
  <tr>
    <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:64px;padding-left:30px;padding-right:30px;padding-top:64px;" class="indented"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="center"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:14px;line-height:28px;text-align:center;">
      Carefully curated by Jay Cuthrell with <a target="_parent" style="color: #3498DB" href="https://www.getrevue.co/?utm_source=Jay Cuthrell&amp;utm_medium=email&amp;utm_content=footerlink&amp;utm_campaign=Issue">Revue</a>.
      If you were forwarded this newsletter and you like it, <a target="_blank" style="color: #3498DB" href="http://digest.jaycuthrell.com/?utm_campaign=Issue&amp;utm_content=forwarded&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">you can subscribe here</a>.
      If you don't want these updates anymore, please unsubscribe
      <a style="color: #3498DB" href="#">here</a>.
    </div></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]--></td></tr></tbody></table></div><!--[if mso | IE]>
</td></tr></table>
<![endif]-->
  </div>
</body>
</html>
</body>
</html>
