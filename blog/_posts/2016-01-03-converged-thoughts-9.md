---
layout: post
title: "Converged Thoughts: Issue 9"
date: 2017-01-03 10:24
redirect_from:
  - /issues/virtual-reality-80s-and-90s-nostalgia-41351
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
<meta name="csrf-token" content="BdGrkmozZTODBU59YIHhWfcCP74pHt5gHgr2QAwqch3HhOeBuWYwjcfvmWFPp2XADDJyTkpYNaw6DbteNT4IDQ==" />

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
      <div style="display:none;font-size:1px;color:#FFF;line-height:1px;max-height:0px;max-width:0px;opacity:0;overflow:hidden;">Yesterday, I had my first immersive VR experience. It was the total package. Headgear. Trackers. Hapt</div>

      
    

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
      Virtual Reality: 80s and 90s Nostalgia
    </div></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="left"><div style="cursor:auto;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:16px;line-height:20px;text-align:left;font-weight:500;color: #9932CC;">
      By <a style="color: #9932CC" href="http://digest.jaycuthrell.com/?utm_campaign=Issue&amp;utm_content=profileimage&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">Jay Cuthrell</a>&nbsp;&bull;&nbsp;Issue #9
    </div></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-top:28px;" align="left"><div style="cursor:auto;color:#3B424B;font-family:Georgia, 'Times New Roman', Times, serif;font-size:18px;line-height:32px;text-align:left;"><div style="margin: 0;" class="revue-p">Yesterday, I had my first immersive VR experience. It was the total package. Headgear. Trackers. Haptics. Consoles. Rigs. Probiotic Yogurt. Honestly, I’m not sure why I waited so long to try this. Yes, my mind was suitably blown.  Let’s start the digesting…</div>

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
<![endif]--><div style="margin:0px auto;max-width:600px;"><table role="presentation" cellpadding="0" cellspacing="0" style="font-size:0px;width:100%;" align="center" border="0"><tbody><tr><td style="text-align:center;vertical-align:top;direction:ltr;font-size:0px;padding:0px;padding-bottom:44px;"><!--[if mso | IE]>
<table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td style="vertical-align:top;width:600px;">
<![endif]--><div aria-labelledby="mj-column-per-100" class="mj-column-per-100 outlook-group-fix" style="vertical-align:top;display:inline-block;direction:ltr;font-size:13px;text-align:left;width:100%;"><table role="presentation" cellpadding="0" cellspacing="0" width="100%" border="0"><tbody><tr><td style="word-break:break-word;font-size:0px;padding:0px;" align="center"><table role="presentation" cellpadding="0" cellspacing="0" style="border-collapse:collapse;border-spacing:0px;" align="center" border="0"><tbody><tr><td style="width:600px;">
    <img alt="" title="" height="auto" src="https://s3.amazonaws.com/revue/items/images/001/669/962/mail/vr.png?1483583582" style="border:none;border-radius:0;display:block;outline:none;text-decoration:none;width:100%;height:auto;" width="600">
</td></tr></tbody></table></td></tr><tr><td style="word-break:break-word;font-size:0px;padding:0px;padding-top:16px;" align="center"><div style="cursor:auto;color:#3B424B;font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif;font-size:14px;line-height:16px;text-align:center;">Picture of the VR advert at Capital Factory in Austin, Texas</div></td></tr></tbody></table></div><!--[if mso | IE]>
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
          <a target="_blank" style="text-decoration: none;" href="https://twitter.com/JayCuthrell/status/816768161123078144?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/670/054/thumb/Jpc0KbFA_400x400.jpg?1483591533" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://twitter.com/JayCuthrell/status/816768161123078144?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Great @CapitalFactory @CFVRLab @OwlchemyLabs demos today.

🤓🕶😎👽

My mind is now officially blown.

AMAZING! #AR #VR 
https://t.co/Sl4W0mwFxY</a></div>        
        
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/owlrY?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">twitter.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/owlrY?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
      Silver Screen SQUID Approximations
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
      <div style="margin: 0;" class="revue-p">Growing up in North Carolina, “Brainstorm” was one of those science fiction movies you heard more about in the local news than you did from people that went to see it in a theater. Most folks I grew up with saw it on HBO when cable came to our neighborhoods. </div><div style="margin: 0;" class="revue-p">Filming locations included all the places that would be part of my youth. The Outer Banks, Research Triangle Park, and various university settings were literally the backdrop for science fiction.</div>

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
          <a target="_blank" style="text-decoration: none;" href="http://www.imdb.com/title/tt0085271/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="left" style="padding-right: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/811/thumb/MV5BMzVlNDIwZjItZDM1NS00NmY5LTk1OGItZTBhYTdkNzM0ZDlhXkEyXkFqcGdeQXVyNDk3NzU2MTQ_._V1_UY1200_CR109_0_630_1200_AL_.jpg?1483576146" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="http://www.imdb.com/title/tt0085271/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Brainstorm (1983) - IMDb</a></div>
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Boy meets Girl. Girl gets her cerebral cortex recorded.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/7OY3A?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.imdb.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/7OY3A?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
          <a target="_blank" style="text-decoration: none;" href="http://www.imdb.com/title/tt0114558/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/812/thumb/MV5BMjQ2NTQ0NzgtODUzYy00NThlLWFhNDEtNjhkY2M0M2EwY2ZmXkEyXkFqcGdeQXVyNDk3NzU2MTQ_._V1_UY1200_CR84_0_630_1200_AL_.jpg?1483576180" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="http://www.imdb.com/title/tt0114558/?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Strange Days (1995) - IMDb</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Enjoy the 900 MHz wireless phones of the “future”.</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/rjlqk?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.imdb.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/rjlqk?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
      <div style="margin: 0;" class="revue-p">“Strange Days” is also science fiction but it is a bit darker and edgier compared to the magical wonder of “Brainstorm”. The filming locations are right in the backyard of Hollywood. Some of those locations I’ve visited in my career.</div><div style="margin: 0;" class="revue-p">Now, are either of these movies about VR? Not exactly.</div><div style="margin: 0;" class="revue-p">In avoiding spoilers, the primary plot device in both movies (for me at least) was the notion of recording and playing back the experiences of the brain using a superconducting quantum interference device (SQUID). Both involved computing and storage device media so as my career has involved computing and storage oriented companies for the past several years – very amusing in retrospect.</div><div style="margin: 0;" class="revue-p">Both movies were a riff on the rise personal media recording starting with the humble VCR of the 80s and the eventual DVD of the 90s. In both tales, a person could record the total immersive experience they are having (their reality) and then that same person OR another person could experience it again – everything see hear smell touch everything – because the SQUID was doing both recording and playback by accessing brainwaves. In effect, this is passive viewing of an immutable and durable experience.</div>

    </div></td></tr></tbody></table></div><!--[if mso | IE]>
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
      Control and the Construct
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
      <div style="margin: 0;" class="revue-p">If you are reading this digest, I’ll go out on a limb and guess that you’ve seen at least one if not all of “The Matrix” trilogy or failing that, perhaps the holodeck from “Star Trek: The Next Generation”.</div>

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
          <a target="_blank" style="text-decoration: none;" href="http://matrix.wikia.com/wiki/Construct?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/906/thumb/latest?1483580757" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="http://matrix.wikia.com/wiki/Construct?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Construct</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">A Construct is a virtual work space or “loading program” created to run simulations or upload…</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/M9qJk?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">matrix.wikia.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/M9qJk?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
          <a target="_blank" style="text-decoration: none;" href="http://memory-alpha.wikia.com/wiki/Holodeck?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">
            <img width="140" height="140" alt="" align="left" style="padding-right: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/911/thumb/latest?1483581342" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="http://memory-alpha.wikia.com/wiki/Holodeck?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue">Holodeck</a></div>
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">A Holographic Environment Simulator, or holodeck for short, was a form of holotechnology…</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/7OY76?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">memory-alpha.wikia.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/7OY76?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
      <div style="margin: 0;" class="revue-p">In terms of where VR is today visually, it’s not “The Matrix” by a long shot. Rather, it’s probably capable of reaching somewhere in the range of “Polar Express” uncanny valley creepy though.</div><div style="margin: 0;" class="revue-p">The experiences will improve as demand generation puts more VR headsets and peripherals into the hands of a new generation of gamer, trainer, and entrepreneur. Combined with advances in computing and networking speeds, things are going to get feisty.</div><div style="margin: 0;" class="revue-p">So, the natural question would be where convergence fits into place. For me, I look back to the SQUID of “Strange Days” and even “Brainstorm”.</div><div style="margin: 0;" class="revue-p">Convergence in VR will be interesting for several areas:</div><div style="margin: 0;" class="revue-p"><br style=""></div><ul style="">
<li style="">High end headsets will be replaced by an affordable SQUID that might not be too far off from donning a fashionable hat (hey, it can’t be worse than when folks were Bluetooth earpieces)</li>
<li style="">Processing units for the VR experience that currently require tower size gaming rigs will be replaced by ultra portable devices</li>
<li style="">A lessening of dependency on the current accoutrements will allow a user to be paired with biologically sound interfaces</li>
<ul style="">
<li style="">sub dermal SQUID</li>
<li style="">haptic implantation</li>
</ul>
<li style="">Software improvements obviating <a href="http://www.imdb.com/title/tt0104692/" style="color: #3498DB" target="_blank">psycotropics</a> (to get past algorithmic challenges for suspension of disbelief) will give rise to blending of VR and augmented reality (AR) without the need for glasses<br style="">
</li>
</ul><div style="margin: 0;" class="revue-p">As for the convergence of the physical impacts of a VR or AR experience I can see a couple of possibilities</div><ol style="">
<li style="">Bounded experience areas requiring a user to stay in a flat grid will be replaced with active surfaces and other logically configured physical environments (approaching the holodeck concept)</li>
<li style="">A passive physical posture will be more desirable and “The Matrix” approach of stimulation will mean the user just stays in a fixed position.</li>
</ol><div style="margin: 0;" class="revue-p">Will experiences be available in a RedBox kiosk like DVDs and games are today? Will experiences be massive downloads like with a movie from Netflix? Will we be able to stream an experience? Can I subscribe to a bundle of experiences? Will experiences have discount codes if I subscribe to a series of experiences on retail’s digital Black Friday?</div><div style="margin: 0;" class="revue-p">These are all great questions to ask. As the consumer experience dictates, the convergence will arrive to satisfy a scenario where “it just works”.</div><div style="margin: 0;" class="revue-p">Lastly, as a reminder… convergence will also apply in how we communicate and share experiences and improve upon the pursuit of refinements in developed skills. It’s already happening now on the edges of the IT and skills continuum. Soon these new training methods will coming to a consumer retail ready experience near you and the people you know and probably sooner than you think.</div>

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
          <a target="_blank" style="text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=oIvdvG_zj6A">
            <img width="140" height="140" alt="" align="right" style="padding-left: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/944/thumb/maxresdefault.jpg?1483582729" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=oIvdvG_zj6A">Enhanced Training Through Neurostimulation</a></div>        
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Soon…</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/3RqKA?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.youtube.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/3RqKA?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
      <div style="margin: 0;" class="revue-p">In fact, yesterday I did some on the job training of my own! This video doesn’t do justice to what I experienced but it gives you an idea of what the possibilities are going to be now and in the very near future.</div>

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
          <a target="_blank" style="text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=6vMO3XmNXe4">
            <img width="140" height="140" alt="" align="left" style="padding-right: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/983/thumb/hqdefault.jpg?1483585718" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=6vMO3XmNXe4">Matrix - I Know Kung Fu</a></div>
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Eventually…</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/9O44Y?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.youtube.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/9O44Y?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
          <a target="_blank" style="text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=Uhh4dA-V2os">
            <img width="140" height="140" alt="" align="left" style="padding-right: 30px; padding-bottom: 36px;border:none;border-radius:0;outline:none;text-decoration:none;" class="link-image" src="https://s3.amazonaws.com/revue/items/images/001/669/950/thumb/maxresdefault.jpg?1483582960" />
</a>        <div class="link-title" style="padding-bottom: 8px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, sans-serif; color: #27285F; font-size: 20px; line-height: 28px; font-weight: 600;"><a target="_blank" style="color: #3498DB; text-decoration: none;" href="https://www.youtube.com/watch?utm_campaign=Revue%20newsletter&amp;utm_medium=Newsletter&amp;utm_source=revue&amp;v=Uhh4dA-V2os">Job Simulator - Office Worker Teaser - Owlchemy Labs</a></div>
        <div class="serif small-text" style="font-family: Georgia, 'Times New Roman', Times, serif; font-size: 16px; line-height: 28px; color: #3B424B; padding-bottom: 8px;"><div style="margin: 0;" class="revue-p">Announcing the third job within Job Simulator - Office Worker. Job Simulator is a tongue-in-cheek virtual reality experience for motion controlled VR platfor…</div>
</div>
        <div class="link-url" style="font-size: 14px; line-height: 16px; color: #9932CC;">
          <a target="_blank" style="text-decoration: none; color: #9932CC;" href="http://rev.vu/M9qmk?utm_campaign=Issue&amp;utm_content=domain&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">www.youtube.com</a>
           &bull; 
          <a target="_blank" style="text-decoration: none; color: #9932CC; text-decoration: none;" href="http://rev.vu/M9qmk?utm_campaign=Issue&amp;utm_content=share&amp;utm_medium=email&amp;utm_source=Jay+Cuthrell">share</a>
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
            <a target="_blank" style="color: #1DA1F2; text-decoration: none;" href="https://www.twitter.com/share?url=http://digest.jaycuthrell.com/archive/41351&amp;via=revue&amp;text=Virtual%20Reality%3A%2080s%20and%2090s%20Nostalgia%20by%20%40JayCuthrell&amp;related=revue">
              <img alt="" width="24" height="20" style="border:none;border-radius:0;outline:none;text-decoration:none;vertical-align:middle;padding-right:3px;" src="//d3jbm9h03wxzi9.cloudfront.net/assets/email/share_twitter_2-c23bb19c3c2dbb4d69a4a5d6630babeab20cda45cf6876450e97cd68b50d2e60.png" />
              <strong style="color: #1DA1F2;vertical-align:middle;">Tweet</strong>
</a>               
            <a target="_blank" style="color: #3B5998; text-decoration: none;" href="http://www.facebook.com/sharer/sharer.php?u=http://digest.jaycuthrell.com/archive/41351">
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
