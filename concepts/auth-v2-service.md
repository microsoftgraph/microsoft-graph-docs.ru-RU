---
title: Получение доступа без пользователя
description: Некоторые приложения вызывают Microsoft Graph от своего имени, а не от имени пользователя. Очень часто это фоновые службы и управляющие программы, которые работают на сервере без выполнившего вход пользователя.
author: jackson-woods
localization_priority: Priority
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 0fba65fb040ca210b5d9a9fe82e9510b5586c4b6
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53333970"
---
# <a name="get-access-without-a-user"></a><span data-ttu-id="98389-104">Получение доступа без пользователя</span><span class="sxs-lookup"><span data-stu-id="98389-104">Get access without a user</span></span>

<span data-ttu-id="98389-p102">Некоторые приложения вызывают Microsoft Graph от своего имени, а не от имени пользователя. Зачастую это фоновые службы и управляющие программы, которые работают на сервере без выполнившего вход пользователя. Примером таких приложений можно назвать службу архивации электронной почты, которая выходит из спящего режима и работает в течение ночи. В некоторых случаях приложения также могут вызывать Microsoft Graph от своего имени, когда пользователь выполнил вход. Например, приложению может потребоваться возможность, для использования которой нужны более высокие привилегии, чем те, которыми обладает пользователь.</span><span class="sxs-lookup"><span data-stu-id="98389-p102">Some apps call Microsoft Graph with their own identity and not on behalf of a user. In many cases, these are background services or daemons that run on a server without the presence of a signed-in user. An example of such an app might be an email archival service that wakes up and runs overnight. In some cases, apps that have a signed-in user present may also need to call Microsoft Graph under their own identity. For example, an app may need to use functionality that requires more elevated privileges in an organization than those carried by the signed-in user.</span></span>  

<span data-ttu-id="98389-p103">Приложения, которые вызывают Microsoft Graph от своего имени, используют [поток предоставления учетных данных клиента](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) OAuth 2.0 для получения маркеров доступа из Azure AD. В этой статье описываются основные действия по настройке службы и использованию потока предоставления учетных данных клиента OAuth, чтобы получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="98389-p103">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 [client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to get access tokens from Azure AD. This topic describes the basic steps to configure a service and use the OAuth client credentials grant flow to get an access token.</span></span>

## <a name="authentication-and-authorization-steps"></a><span data-ttu-id="98389-112">Этапы аутентификации и авторизации</span><span class="sxs-lookup"><span data-stu-id="98389-112">Authentication and authorization steps</span></span>

<span data-ttu-id="98389-113">Чтобы настроить службу и получить маркер из конечной точки платформы удостоверений Майкрософт, необходимый службе для вызова Microsoft Graph от своего имени, нужно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="98389-113">The basic steps required to configure a service and get a token from the Microsoft identity platform endpoint that your service can use to call Microsoft Graph under its own identity are:</span></span>

1. <span data-ttu-id="98389-114">Регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="98389-114">Register your app.</span></span>
2. <span data-ttu-id="98389-115">Настройка разрешений для Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="98389-115">Configure permissions for Microsoft Graph on your app.</span></span>
3. <span data-ttu-id="98389-116">Получение согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="98389-116">Get administrator consent.</span></span>
4. <span data-ttu-id="98389-117">Получение маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="98389-117">Get an access token.</span></span>
5. <span data-ttu-id="98389-118">Вызов Microsoft Graph с помощью маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="98389-118">Use the access token to call Microsoft Graph.</span></span>

## <a name="1-register-your-app"></a><span data-ttu-id="98389-119">1. Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="98389-119">1. Register your app</span></span>

<span data-ttu-id="98389-p104">Чтобы обеспечить прохождение проверки подлинности в конечной точке платформы удостоверений Майкрософт, необходимо сначала зарегистрировать приложение на [портале Azure для регистрации приложений](https://go.microsoft.com/fwlink/?linkid=2083908). Для регистрации приложения можно использовать либо учетную запись Майкрософт, либо рабочую или учебную учетную запись.</span><span class="sxs-lookup"><span data-stu-id="98389-p104">To authenticate with the Microsoft identity platform endpoint, you must first register your app at the [Azure app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908). You can use either a Microsoft account or a work or school account to register your app.</span></span>

<span data-ttu-id="98389-122">Чтобы служба могла вызывать Microsoft Graph от своего имени, вам нужно зарегистрировать приложение для веб-платформы и скопировать следующие значения:</span><span class="sxs-lookup"><span data-stu-id="98389-122">For a service that will call Microsoft Graph under its own identity, you need to register your app for the Web platform and copy the following values:</span></span>

- <span data-ttu-id="98389-123">идентификатор приложения, назначенный порталом регистрации Azure;</span><span class="sxs-lookup"><span data-stu-id="98389-123">The Application ID assigned by the Azure app registration portal.</span></span>
- <span data-ttu-id="98389-124">секрет клиента (приложения) — пароль либо открытый и закрытый ключ (сертификат);</span><span class="sxs-lookup"><span data-stu-id="98389-124">A Client (application) Secret, either a password or a public/private key pair (certificate).</span></span>
- <span data-ttu-id="98389-125">URL-адрес перенаправления, с помощью которого служба будет получать ответы с маркерами;</span><span class="sxs-lookup"><span data-stu-id="98389-125">A Redirect URL for your service to receive token responses.</span></span>
- <span data-ttu-id="98389-126">URL-адрес перенаправления, с помощью которого служба будет получать ответы с согласием администратора, если в приложении реализованы функции для запроса согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="98389-126">A Redirect URL for your service to receive admin consent responses if your app implements functionality to request administrator consent.</span></span>  

<span data-ttu-id="98389-127">Инструкции по настройке приложения на портале Azure см. в статье [Регистрация приложения](./auth-register-app-v2.md).</span><span class="sxs-lookup"><span data-stu-id="98389-127">For steps on how to configure an app using the Azure app registration portal, see [Register your app](./auth-register-app-v2.md).</span></span>

<span data-ttu-id="98389-128">Когда используется поток предоставления учетных данных клиента OAuth 2.0, приложение проходит аутентификацию непосредственно в конечной точке `/token` платформы удостоверений Майкрософт, используя идентификатор приложения, назначенный службой Azure AD, и секрет приложения, созданный вами на портале.</span><span class="sxs-lookup"><span data-stu-id="98389-128">With the OAuth 2.0 client credentials grant flow, your app authenticates directly at the Microsoft identity platform `/token` endpoint using the Application ID assigned by Azure AD and the Application Secret that you create using the portal.</span></span>

## <a name="2-configure-permissions-for-microsoft-graph"></a><span data-ttu-id="98389-129">2. Настройка разрешений для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="98389-129">2. Configure permissions for Microsoft Graph</span></span>

<span data-ttu-id="98389-p105">Для приложений, вызывающих Microsoft Graph от своего имени, Microsoft Graph предоставляет специальные разрешения. (Microsoft Graph также может предоставлять делегированные разрешения для приложений, вызывающих Microsoft Graph от имени пользователя.) Предварительная настройка разрешений приложения, необходимых вашему приложению, выполняется при его регистрации. Разрешения приложения всегда требуют согласия администратора. Администратор может согласиться предоставить эти разрешения на [портале Azure](https://portal.azure.com) во время установки приложения в организации. Вы также можете создать в приложении интерфейс регистрации, где администраторы могут соглашаться на предоставление заданных вами разрешений. Когда согласие администратора фиксируется в Azure AD, приложение может запрашивать маркеры, не требуя повторного согласия. Дополнительные сведения о разрешениях, доступных в Microsoft Graph, см. в [справочнике по разрешениям](./permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="98389-p105">For apps that call Microsoft Graph under their own identity, Microsoft Graph exposes application permissions (Microsoft Graph can also expose delegated permissions for apps that call Microsoft Graph on behalf of a user). You pre-configure the application permissions your app needs when you register your app. Application permissions always require administrator consent. An administrator can either consent to these permissions using the [Azure portal](https://portal.azure.com) when your app is installed in their organization, or you can provide a sign-up experience in your app through which administrators can consent to the permissions you configured. Once administrator consent is recorded by Azure AD, your app can request tokens without having to request consent again. For more detailed information about the permissions available with Microsoft Graph, see the [Permissions reference](./permissions-reference.md)</span></span>

<span data-ttu-id="98389-136">Настроить разрешения приложения, необходимые вашему приложению, можно на [портале Azure для регистрации приложений](https://go.microsoft.com/fwlink/?linkid=2083908). Откройте страницу **Разрешения API** для приложения, нажмите кнопку **Добавить разрешение**, выберите **Microsoft Graph**, а затем выберите нужные разрешения в разделе **Разрешения приложения**.</span><span class="sxs-lookup"><span data-stu-id="98389-136">To configure application permissions for your app in the [Azure app registrations portal](https://go.microsoft.com/fwlink/?linkid=2083908): under an application's **API permissions** page, choose **Add a permission**, select **Microsoft Graph**, and then choose the permissions your app requires under **Application permissions**.</span></span>

<span data-ttu-id="98389-137">На приведенном ниже снимке экрана показано диалоговое окно **Выбор разрешений** с разрешениями приложения в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="98389-137">The following screenshot shows the **Select Permissions** dialog box for Microsoft Graph application permissions.</span></span>

![Диалоговое окно "Выбор разрешений" с разрешениями приложения в Microsoft Graph.](./images/auth-v2/v2-application-permissions.png)

> <span data-ttu-id="98389-p106">**Примечание.** Рекомендуем настроить минимальный набор разрешений, необходимый приложению. Это намного удобнее для администраторов, чем необходимость соглашаться на длинный список разрешений.</span><span class="sxs-lookup"><span data-stu-id="98389-p106">**Note**: We recommend that you configure the least privileged set of permissions required by your app. This provides a much more comfortable experience for administrators than having to consent to a long list of permissions.</span></span>

## <a name="3-get-administrator-consent"></a><span data-ttu-id="98389-141">3. Получение согласия администратора</span><span class="sxs-lookup"><span data-stu-id="98389-141">3. Get administrator consent</span></span>

<span data-ttu-id="98389-142">Вы можете рассчитывать на то, что администратор предоставит разрешения, необходимые приложению, на [портале Azure](https://portal.azure.com). Однако зачастую лучший вариант — предоставить администраторам возможность регистрации с помощью конечной точки `/adminconsent` платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="98389-142">You can rely on an administrator to grant the permissions your app needs at the [Azure portal](https://portal.azure.com); however, often, a better option is to provide a sign-up experience for administrators by using the Microsoft identity platform `/adminconsent` endpoint.</span></span> 

> <span data-ttu-id="98389-143">**Важно!** Когда вы вносите изменение в настроенные разрешения, их должен заново подтвердить администратор.</span><span class="sxs-lookup"><span data-stu-id="98389-143">**Important**: Any time you make a change to the configured permissions, you must also repeat the Admin Consent process.</span></span> <span data-ttu-id="98389-144">Изменения, внесенные на портале регистрации приложений, не вступят в силу, пока их не подтвердит администратор клиента.</span><span class="sxs-lookup"><span data-stu-id="98389-144">Changes made in the app registration portal will not be reflected until consent has been reapplied by the tenant's administrator.</span></span>

### <a name="request"></a><span data-ttu-id="98389-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="98389-145">Request</span></span>

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=https://localhost/myapp/permissions
```

| <span data-ttu-id="98389-146">Параметр</span><span class="sxs-lookup"><span data-stu-id="98389-146">Parameter</span></span>     | <span data-ttu-id="98389-147">Условие</span><span class="sxs-lookup"><span data-stu-id="98389-147">Condition</span></span>   | <span data-ttu-id="98389-148">Описание</span><span class="sxs-lookup"><span data-stu-id="98389-148">Description</span></span> 
|:--------------|:------------|:------------
| <span data-ttu-id="98389-149">tenant</span><span class="sxs-lookup"><span data-stu-id="98389-149">tenant</span></span>        | <span data-ttu-id="98389-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-150">Required</span></span>    | <span data-ttu-id="98389-p108">Клиент каталога, у которого требуется запрашивать разрешения. Он может быть представлен в виде GUID или в формате понятного имени. Если вы не знаете, к какому клиенту относится пользователь, и хотите, чтобы он мог войти в любой клиент, используйте значение `common`.</span><span class="sxs-lookup"><span data-stu-id="98389-p108">The directory tenant that you want to request permission from. This can be in GUID or friendly name format. If you don't know which tenant the user belongs to and you want to let them sign in with any tenant, use `common`.</span></span>
| <span data-ttu-id="98389-154">client_id</span><span class="sxs-lookup"><span data-stu-id="98389-154">client_id</span></span>     | <span data-ttu-id="98389-155">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-155">Required</span></span>    | <span data-ttu-id="98389-156">Идентификатор приложения, назначенный [порталом Azure для регистрации приложений](https://go.microsoft.com/fwlink/?linkid=2083908).</span><span class="sxs-lookup"><span data-stu-id="98389-156">The Application ID that the [Azure app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908) assigned to your app.</span></span>
| <span data-ttu-id="98389-157">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="98389-157">redirect_uri</span></span>  | <span data-ttu-id="98389-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-158">Required</span></span>    | <span data-ttu-id="98389-p109">URI перенаправления, на который должен отправляться ответ для обработки приложением. Он должен в точности совпадать с одним из URI перенаправления, зарегистрированных на портале, и быть закодирован как URL-адрес. Может содержать дополнительные сегменты пути.</span><span class="sxs-lookup"><span data-stu-id="98389-p109">The redirect URI where you want the response to be sent for your app to handle. It must exactly match one of the redirect URIs that you registered in the portal, except that it must be URL encoded, and it can have additional path segments.</span></span>
| <span data-ttu-id="98389-161">state</span><span class="sxs-lookup"><span data-stu-id="98389-161">state</span></span>         | <span data-ttu-id="98389-162">Рекомендуемый</span><span class="sxs-lookup"><span data-stu-id="98389-162">Recommended</span></span> | <span data-ttu-id="98389-p110">Значение, которое включается в запрос и возвращается в ответе с маркером. Это может быть строка с любым содержимым. Параметр state используется для кодирования сведений о состоянии пользователя в приложении до запрашивания проверки подлинности, например о просматриваемых странице и представлении.</span><span class="sxs-lookup"><span data-stu-id="98389-p110">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span>

### <a name="administrator-consent-experience"></a><span data-ttu-id="98389-166">Предоставление согласия администратора</span><span class="sxs-lookup"><span data-stu-id="98389-166">Administrator consent experience</span></span>

<span data-ttu-id="98389-p111">В Azure AD действует правило, что только администратор клиента может подтвердить запрос к конечной точке `/adminconsent`. Администратору будет предложено утвердить все разрешения для приложения, запрошенные вами на портале регистрации.</span><span class="sxs-lookup"><span data-stu-id="98389-p111">With requests to the `/adminconsent` endpoint, Azure AD enforces that only a tenant administrator can sign in to complete the request. The administrator will be asked to approve all the application permissions that you have requested for your app in the app registration portal.</span></span>

<span data-ttu-id="98389-169">Ниже представлен пример диалогового окна предоставления согласия, которое Azure AD отображает для администратора.</span><span class="sxs-lookup"><span data-stu-id="98389-169">The following is an example of the consent dialog that Azure AD presents to the administrator:</span></span>

![Диалоговое окно согласия администратора.](./images/admin-consent.png)

### <a name="response"></a><span data-ttu-id="98389-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="98389-171">Response</span></span>

<span data-ttu-id="98389-172">Если администратор утверждает разрешения для приложения, успешный ответ выглядит так:</span><span class="sxs-lookup"><span data-stu-id="98389-172">If the administrator approves the permissions for your application, the successful response looks like this:</span></span>

```
// Line breaks are for legibility only.

GET https://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| <span data-ttu-id="98389-173">Параметр</span><span class="sxs-lookup"><span data-stu-id="98389-173">Parameter</span></span>     | <span data-ttu-id="98389-174">Описание</span><span class="sxs-lookup"><span data-stu-id="98389-174">Description</span></span>
|:--------------|:------------
| <span data-ttu-id="98389-175">tenant</span><span class="sxs-lookup"><span data-stu-id="98389-175">tenant</span></span>        | <span data-ttu-id="98389-176">Клиент каталога, который предоставил приложению запрашиваемые разрешения, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="98389-176">The directory tenant that granted your application the permissions that it requested, in GUID format.</span></span>
| <span data-ttu-id="98389-177">state</span><span class="sxs-lookup"><span data-stu-id="98389-177">state</span></span>         | <span data-ttu-id="98389-p112">Значение, которое включается в запрос и возвращается в ответе с маркером. Это может быть строка с любым содержимым. Параметр state используется для кодирования сведений о состоянии пользователя в приложении до запрашивания проверки подлинности, например о просматриваемых странице и представлении.</span><span class="sxs-lookup"><span data-stu-id="98389-p112">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span>
| <span data-ttu-id="98389-181">admin_consent</span><span class="sxs-lookup"><span data-stu-id="98389-181">admin_consent</span></span> | <span data-ttu-id="98389-182">Задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="98389-182">Set to **true**.</span></span>


> <span data-ttu-id="98389-p113">**Попробуйте**. Вы можете проверить это самостоятельно, вставив приведенный ниже запрос в браузер. Если вы войдете как глобальный администратор клиента Azure AD, откроется диалоговое окно предоставления разрешений для приложения. Это будет другое приложение (не то, что показано на снимке экрана выше).</span><span class="sxs-lookup"><span data-stu-id="98389-p113">**Try**: You can try this for yourself by pasting the following request in a browser. If you sign in as a Global administrator for an Azure AD tenant, you will be presented with the administrator consent dialog box for the app. (This will be a different app than that in the consent dialog box screenshot shown earlier.)</span></span>
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a><span data-ttu-id="98389-186">4. Получение маркера доступа</span><span class="sxs-lookup"><span data-stu-id="98389-186">4. Get an access token</span></span>

<span data-ttu-id="98389-187">В потоке предоставления учетных данных клиента OAuth 2.0 вы используете идентификатор и секрет приложения, сохраненные во время его регистрации, чтобы запросить маркер доступа непосредственно из конечной точки `/token` платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="98389-187">In the OAuth 2.0 client credentials grant flow, you use the Application ID and Application Secret values that you saved when you registered your app to request an access token directly from the Microsoft identity platform `/token` endpoint.</span></span>

<span data-ttu-id="98389-p114">Чтобы указать заранее настроенные разрешения, передайте значение `https://graph.microsoft.com/.default` для параметра `scope` в запросе на получение маркера. Дополнительные сведения см. в описании параметра `scope` в приведенном ниже запросе на получение маркера.</span><span class="sxs-lookup"><span data-stu-id="98389-p114">You specify the pre-configured permissions by passing `https://graph.microsoft.com/.default` as the value for the `scope` parameter in the token request. See the `scope` parameter description in the token request below for details.</span></span>

### <a name="token-request"></a><span data-ttu-id="98389-190">Запрос на получение маркера</span><span class="sxs-lookup"><span data-stu-id="98389-190">Token request</span></span>

<span data-ttu-id="98389-191">Чтобы получить маркер доступа, конечной точке `/token` платформы удостоверений отправляется запрос POST.</span><span class="sxs-lookup"><span data-stu-id="98389-191">You send a POST request to the `/token` identity platform endpoint to acquire an access token:</span></span>

```
// Line breaks are for legibility only.

POST https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=535fb089-9ff3-47b6-9bfb-4f1264799865
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default
&client_secret=qWgdYAmab0YSkuL1qKv5bPX
&grant_type=client_credentials
```

| <span data-ttu-id="98389-192">Параметр</span><span class="sxs-lookup"><span data-stu-id="98389-192">Parameter</span></span>     | <span data-ttu-id="98389-193">Условие</span><span class="sxs-lookup"><span data-stu-id="98389-193">Condition</span></span> | <span data-ttu-id="98389-194">Описание</span><span class="sxs-lookup"><span data-stu-id="98389-194">Description</span></span> 
|:--------------|:----------|:------------
| <span data-ttu-id="98389-195">tenant</span><span class="sxs-lookup"><span data-stu-id="98389-195">tenant</span></span>        | <span data-ttu-id="98389-196">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-196">Required</span></span>  | <span data-ttu-id="98389-p115">Клиент каталога, у которого требуется запрашивать разрешения. Он может быть представлен в виде GUID или в формате понятного имени.</span><span class="sxs-lookup"><span data-stu-id="98389-p115">The directory tenant that you want to request permission from. This can be in GUID or friendly name format.</span></span>
| <span data-ttu-id="98389-199">client_id</span><span class="sxs-lookup"><span data-stu-id="98389-199">client_id</span></span>     | <span data-ttu-id="98389-200">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-200">Required</span></span>  | <span data-ttu-id="98389-201">Идентификатор приложения, назначенный [порталом Azure для регистрации приложений](https://go.microsoft.com/fwlink/?linkid=2083908) при регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="98389-201">The Application ID that the [Azure app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908) assigned when you registered your app.</span></span>
| <span data-ttu-id="98389-202">область</span><span class="sxs-lookup"><span data-stu-id="98389-202">scope</span></span>         | <span data-ttu-id="98389-203">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-203">Required</span></span>  | <span data-ttu-id="98389-204">Значение, передаваемое параметру `scope` этого запроса, должно представлять собой идентификатор (URI идентификатора приложения) нужного ресурса, дополненный суффиксом `.default`.</span><span class="sxs-lookup"><span data-stu-id="98389-204">The value passed for the `scope` parameter in this request should be the resource identifier (Application ID URI) of the resource you want, affixed with the `.default` suffix.</span></span> <span data-ttu-id="98389-205">Для Microsoft Graph используется значение `https://graph.microsoft.com/.default`.</span><span class="sxs-lookup"><span data-stu-id="98389-205">For Microsoft Graph, the value is `https://graph.microsoft.com/.default`.</span></span> <span data-ttu-id="98389-206">Это значение сообщает конечной точке платформы удостоверений Майкрософт, что из всех разрешений приложения, которые вы настроили для своего приложения на портале регистрации приложений, следует выдать маркер для тех, которые связаны с нужным ресурсом.</span><span class="sxs-lookup"><span data-stu-id="98389-206">This value informs the Microsoft identity platform endpoint that of all the application permissions you have configured for your app in the app registration portal, it should issue a token for the ones associated with the resource you want to use.</span></span>
| <span data-ttu-id="98389-207">client_secret</span><span class="sxs-lookup"><span data-stu-id="98389-207">client_secret</span></span> | <span data-ttu-id="98389-208">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-208">Required</span></span>  | <span data-ttu-id="98389-p117">Секрет приложения, созданный на портале регистрации приложений. Используйте зашифрованный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="98389-p117">The Application Secret that you generated for your app in the app registration portal. Ensure that it is URL encoded.</span></span>
| <span data-ttu-id="98389-211">grant_type</span><span class="sxs-lookup"><span data-stu-id="98389-211">grant_type</span></span>    | <span data-ttu-id="98389-212">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98389-212">Required</span></span>  | <span data-ttu-id="98389-213">Должно быть задано значение `client_credentials`.</span><span class="sxs-lookup"><span data-stu-id="98389-213">Must be `client_credentials`.</span></span>

#### <a name="token-response"></a><span data-ttu-id="98389-214">Ответ с маркером</span><span class="sxs-lookup"><span data-stu-id="98389-214">Token response</span></span>

<span data-ttu-id="98389-215">Успешный ответ выглядит так:</span><span class="sxs-lookup"><span data-stu-id="98389-215">A successful response looks like this:</span></span>

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| <span data-ttu-id="98389-216">Параметр</span><span class="sxs-lookup"><span data-stu-id="98389-216">Parameter</span></span>     | <span data-ttu-id="98389-217">Описание</span><span class="sxs-lookup"><span data-stu-id="98389-217">Description</span></span>
|:--------------|:------------
| <span data-ttu-id="98389-218">access_token</span><span class="sxs-lookup"><span data-stu-id="98389-218">access_token</span></span>  | <span data-ttu-id="98389-p118">Запрашиваемый маркер доступа. Приложение может использовать его в вызовах Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="98389-p118">The requested access token. Your app can use this token in calls to Microsoft Graph.</span></span>
| <span data-ttu-id="98389-221">token_type</span><span class="sxs-lookup"><span data-stu-id="98389-221">token_type</span></span>    | <span data-ttu-id="98389-p119">Указывает значение типа маркера. Azure AD поддерживает только тип `bearer`.</span><span class="sxs-lookup"><span data-stu-id="98389-p119">Indicates the token type value. The only type that Azure AD supports is `bearer`.</span></span>
| <span data-ttu-id="98389-224">expires_in</span><span class="sxs-lookup"><span data-stu-id="98389-224">expires_in</span></span>    | <span data-ttu-id="98389-225">Срок действия маркера доступа (в секундах).</span><span class="sxs-lookup"><span data-stu-id="98389-225">How long the access token is valid (in seconds).</span></span>

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a><span data-ttu-id="98389-226">5. Вызов Microsoft Graph с помощью маркера доступа</span><span class="sxs-lookup"><span data-stu-id="98389-226">5. Use the access token to call Microsoft Graph</span></span>

<span data-ttu-id="98389-p120">Получив маркер доступа, вы можете вызвать Microsoft Graph, включив его в заголовок `Authorization` запроса. Приведенный ниже запрос получает профиль определенного пользователя. Для вызова этого API приложению необходимо разрешение _User.Read.All_.</span><span class="sxs-lookup"><span data-stu-id="98389-p120">After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of a specific user. Your app must have the _User.Read.All_ permission to call this API.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
<span data-ttu-id="98389-230">Успешный ответ выглядит примерно так (некоторые заголовки были удалены):</span><span class="sxs-lookup"><span data-stu-id="98389-230">A successful response will look similar to this (some response headers have been removed):</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 309.0273
Date: Wed, 26 Apr 2017 19:53:49 GMT
Content-Length: 407
```

```json
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="supported-app-scenarios-and-resources"></a><span data-ttu-id="98389-231">Поддерживаемые сценарии приложений и ресурсы</span><span class="sxs-lookup"><span data-stu-id="98389-231">Supported app scenarios and resources</span></span>

<span data-ttu-id="98389-232">Приложения, вызывающие Microsoft Graph от своего имени, делятся на две категории:</span><span class="sxs-lookup"><span data-stu-id="98389-232">Apps that call Microsoft Graph under their own identity fall into one of two categories:</span></span>

- <span data-ttu-id="98389-233">[Фоновые службы (управляющие программы)](/azure/active-directory/develop/scenario-daemon-overview), которые работают на сервере без выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="98389-233">[Background services (daemons)](/azure/active-directory/develop/scenario-daemon-overview) that run on a server without a signed-in user.</span></span>
- <span data-ttu-id="98389-234">Приложения также могут вызывать Microsoft Graph от своего имени, если пользователь выполнил вход, например для использования функций, требующих более высоких привилегий, чем те, которыми обладает пользователь.</span><span class="sxs-lookup"><span data-stu-id="98389-234">Apps that have a signed-in user but also call Microsoft Graph with their own identity; for example, to use functionality that requires more elevated privileges than those of the user.</span></span>

<span data-ttu-id="98389-p121">Приложения, которые вызывают Microsoft Graph от своего имени, используют поток предоставления учетных данных клиента OAuth 2.0, чтобы пройти аутентификацию в Azure AD и получить маркер. В случае конечной точки платформы удостоверений Майкрософт вы можете подробнее исследовать этот сценарий с помощью указанных ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="98389-p121">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 client credentials grant to authenticate with Azure AD and get a token. For the Microsoft identity platform endpoint, you can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="98389-237">Более полный вариант потока предоставления учетных данных клиента, который также включает отклики с сообщениями об ошибках, см. в статье [Azure Active Directory версии 2.0 и поток учетных данных клиента OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="98389-237">For a more complete treatment of the client credentials grant flow that also includes error responses, see [Azure Active Directory v2.0 and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>
- <span data-ttu-id="98389-238">Пример вызова Microsoft Graph из службы представлен в [образце управляющей программы версии 2.0](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="98389-238">For a sample that calls Microsoft Graph from a service, see the [v2.0 daemon sample](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) on GitHub.</span></span>
- <span data-ttu-id="98389-239">Дополнительные сведения о рекомендуемых библиотеках проверки подлинности (как от корпорации Майкрософт, так и от сторонних разработчиков) см. в статье [Библиотеки проверки подлинности платформы удостоверений Майкрософт](/azure/active-directory/develop/reference-v2-libraries).</span><span class="sxs-lookup"><span data-stu-id="98389-239">For more information about recommended Microsoft and third-party authentication libraries, see [Microsoft identity platform authentication libraries](/azure/active-directory/develop/reference-v2-libraries).</span></span>

## <a name="endpoint-considerations"></a><span data-ttu-id="98389-240">Рекомендации, связанные с конечной точкой</span><span class="sxs-lookup"><span data-stu-id="98389-240">Endpoint considerations</span></span>

<span data-ttu-id="98389-241">Корпорация Майкрософт продолжает поддерживать конечную точку Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98389-241">Microsoft continues to support the Azure AD endpoint.</span></span> <span data-ttu-id="98389-242">Существует [ряд отличий](/azure/active-directory/develop/azure-ad-endpoint-comparison) между конечной точкой платформы удостоверений Майкрософт и конечной точкой Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98389-242">There are [several differences](/azure/active-directory/develop/azure-ad-endpoint-comparison) between using the Microsoft identity platform endpoint and the Azure AD endpoint.</span></span> <span data-ttu-id="98389-243">При использовании конечной точки Azure AD:</span><span class="sxs-lookup"><span data-stu-id="98389-243">When using the Azure AD endpoint:</span></span>

- <span data-ttu-id="98389-244">Если приложение поддерживается несколькими клиентами, необходимо в явной форме настроить его в таком качестве на [портале Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="98389-244">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant in the [Azure portal](https://portal.azure.com).</span></span>
- <span data-ttu-id="98389-p123">Конечная точка согласия администратора (`/adminconsent`) отсутствует. Вместо этого приложение может запрашивать согласие администратора, добавляя параметр `prompt=admin_consent` к запросу на авторизацию. Дополнительные сведения см. в разделе **Активация инфраструктуры согласия Azure AD во время выполнения** статьи [Интеграция приложений с Azure Active Directory](/azure/active-directory/develop/active-directory-integrating-applications).</span><span class="sxs-lookup"><span data-stu-id="98389-p123">There is no admin consent endpoint (`/adminconsent`). Instead, your app can request administrator consent during runtime by adding the `prompt=admin_consent` parameter to an authorization request. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](/azure/active-directory/develop/active-directory-integrating-applications).</span></span>
- <span data-ttu-id="98389-p124">В запросах на авторизацию и получение маркеров используются другие параметры. Например, в запросах конечной точки Azure AD нет параметра `scope`. Вместо него используется параметр `resource`, чтобы указать URI ресурса (`resource=https://graph.microsoft.com`), для которого запрашивается маркер авторизации (для согласия администратора).</span><span class="sxs-lookup"><span data-stu-id="98389-p124">The parameters in authorization and token requests are different. For example, there is no `scope` parameter in Azure AD endpoint requests; instead, the `resource` parameter is used to specify the URI of the resource (`resource=https://graph.microsoft.com`) that authorization (for administrator consent) or a token is being requested for.</span></span>

<span data-ttu-id="98389-250">Чтобы подробнее изучить этот сценарий, используйте следующие материалы:</span><span class="sxs-lookup"><span data-stu-id="98389-250">You can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="98389-251">Дополнительные сведения об использовании платформы удостоверений Майкрософт для различных типов приложений см. по ссылкам **Начало работы** в [документации по платформе удостоверений Майкрософт](/azure/active-directory/develop/active-directory-developers-guide).</span><span class="sxs-lookup"><span data-stu-id="98389-251">For information about using the Microsoft identity platform with different kinds of apps, see the **Get Started** links in the [Microsoft identity platform documentation](/azure/active-directory/develop/active-directory-developers-guide).</span></span> <span data-ttu-id="98389-252">Руководство содержит ссылки на обзорные статьи, краткие руководства, учебники, примеры кода и документацию по протоколам для различных типов приложений, поддерживаемых платформой удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="98389-252">The guide contains links to overview topics, quickstarts, tutorials, code samples, and protocol documentation for different kinds of apps supported by the Microsoft identity platform.</span></span>
- <span data-ttu-id="98389-253">Сведения о библиотеке проверки подлинности Майкрософт (MSAL) и серверном ПО промежуточного слоя, доступном для использования с конечной точкой платформы удостоверений Майкрософт, см. в статье [Библиотеки проверки подлинности Майкрософт](/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="98389-253">For information about the Microsoft Authentication Library (MSAL) and server middleware available for use with the Microsoft identity platform endpoint, see [Microsoft Authentication Libraries](/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>


## <a name="see-also"></a><span data-ttu-id="98389-254">См. также</span><span class="sxs-lookup"><span data-stu-id="98389-254">See also</span></span>

- <span data-ttu-id="98389-255">Пример веб-приложения, размещаемого в службе приложений Azure, которое вызывает Microsoft Graph в качестве приложения (с помощью управляемых удостоверений), см. в разделе [Учебник. Доступ к Microsoft Graph из защищенного приложения](/azure/app-service/scenario-secure-app-access-microsoft-graph-as-app).</span><span class="sxs-lookup"><span data-stu-id="98389-255">For an example of a web app hosted on Azure App Service calling Microsoft Graph as the app (using managed identities), see [Tutorial: Access Microsoft Graph from a secured app as the app](/azure/app-service/scenario-secure-app-access-microsoft-graph-as-app).</span></span> <span data-ttu-id="98389-256">В этом руководстве показано, как создать в веб-приложении управляемое удостоверение, назначенное системой, добавить разрешения API Microsoft Graph к управляемому удостоверению и вызвать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="98389-256">This tutorial shows you how to create a system-assigned managed identity on a web app, add Microsoft Graph API permissions to a managed identity, and call Microsoft Graph.</span></span>
- <span data-ttu-id="98389-257">Примеры использования платформы удостоверений Майкрософт для защиты различных типов приложений см. в статье [Примеры кода платформы удостоверений Майкрософт (конечная точка 2.0)](/azure/active-directory/develop/sample-v2-code).</span><span class="sxs-lookup"><span data-stu-id="98389-257">For samples using the Microsoft identity platform to secure different application types, see [Microsoft identity platform code samples (v2.0 endpoint)](/azure/active-directory/develop/sample-v2-code).</span></span>
