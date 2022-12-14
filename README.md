# helper-functions

## Set cookie value as a json object in vanilla JS
<code>
document.cookie = `name=${encodeURIComponent(
      JSON.stringify(data)
    )}; expires=${expireTime}; path=${path}`;
</code>

## Retrieve cookie in vanilla JS

<code>
const getCookieValue = (name) =>
    document.cookie.match("(^|;)\\s*" + name + "\\s*=\\s*([^;]+)")?.pop() || "";
</code>
