---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d10ffe883b316449a0b0fb58d57dd018e4e395ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958176"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="c6ad9-103">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c6ad9-103">Update servicePrincipal</span></span>

<span data-ttu-id="c6ad9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6ad9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6ad9-105">Обновление свойств объекта [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c6ad9-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c6ad9-106">Использование метода PATCH для настройки [**passwordCredential**](../resources/passwordcredential.md) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="c6ad9-107">Используйте методы [addPassword](./serviceprincipal-addpassword.md) и [removePassword](./serviceprincipal-removepassword.md) для обновления пароля для servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-107">Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6ad9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ad9-108">Permissions</span></span>
<span data-ttu-id="c6ad9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6ad9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6ad9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ad9-111">Permission type</span></span>      | <span data-ttu-id="c6ad9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6ad9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6ad9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6ad9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6ad9-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6ad9-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6ad9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6ad9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6ad9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-116">Not supported.</span></span>    |
|<span data-ttu-id="c6ad9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6ad9-117">Application</span></span> | <span data-ttu-id="c6ad9-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6ad9-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6ad9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6ad9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c6ad9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6ad9-120">Request headers</span></span>
| <span data-ttu-id="c6ad9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6ad9-121">Name</span></span>       | <span data-ttu-id="c6ad9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ad9-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c6ad9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6ad9-123">Authorization</span></span> | <span data-ttu-id="c6ad9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6ad9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6ad9-126">Content-Type</span></span> | <span data-ttu-id="c6ad9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6ad9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6ad9-129">Request body</span></span>
<span data-ttu-id="c6ad9-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c6ad9-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6ad9-133">Property</span></span>     | <span data-ttu-id="c6ad9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c6ad9-134">Type</span></span> |<span data-ttu-id="c6ad9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ad9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ad9-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="c6ad9-136">accountEnabled</span></span>|<span data-ttu-id="c6ad9-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6ad9-137">Boolean</span></span>| <span data-ttu-id="c6ad9-138">Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
|<span data-ttu-id="c6ad9-139">addIns</span><span class="sxs-lookup"><span data-stu-id="c6ad9-139">addIns</span></span>| [<span data-ttu-id="c6ad9-140">addIn</span><span class="sxs-lookup"><span data-stu-id="c6ad9-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="c6ad9-141">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-141">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="c6ad9-142">Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler".</span><span class="sxs-lookup"><span data-stu-id="c6ad9-142">For example, applications that can render file streams [may set the addIns property](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="c6ad9-143">Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-143">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="c6ad9-144">alternativeNames</span><span class="sxs-lookup"><span data-stu-id="c6ad9-144">alternativeNames</span></span>|<span data-ttu-id="c6ad9-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c6ad9-145">String collection</span></span>| <span data-ttu-id="c6ad9-146">Используется для получения субъектов-служб по подпискам, для идентификации групп ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).</span><span class="sxs-lookup"><span data-stu-id="c6ad9-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="c6ad9-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="c6ad9-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="c6ad9-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6ad9-148">Boolean</span></span>|<span data-ttu-id="c6ad9-149">Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-149">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span> <span data-ttu-id="c6ad9-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-150">Not nullable.</span></span> |
|<span data-ttu-id="c6ad9-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="c6ad9-151">appRoles</span></span>|<span data-ttu-id="c6ad9-152">Коллекция [appRole](../resources/approle.md)</span><span class="sxs-lookup"><span data-stu-id="c6ad9-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="c6ad9-153">Роли приложения, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-153">The application roles exposed by the associated application.</span></span> <span data-ttu-id="c6ad9-154">Дополнительные сведения см. в определении свойства **appRoles** для ресурса [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="c6ad9-154">For more information see the **appRoles** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="c6ad9-155">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-155">Not nullable.</span></span> |
|<span data-ttu-id="c6ad9-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c6ad9-156">displayName</span></span>|<span data-ttu-id="c6ad9-157">String</span><span class="sxs-lookup"><span data-stu-id="c6ad9-157">String</span></span>|<span data-ttu-id="c6ad9-158">Отображаемое имя для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="c6ad9-159">homepage</span><span class="sxs-lookup"><span data-stu-id="c6ad9-159">homepage</span></span>|<span data-ttu-id="c6ad9-160">String</span><span class="sxs-lookup"><span data-stu-id="c6ad9-160">String</span></span>|<span data-ttu-id="c6ad9-161">Главная или начальная страница приложения.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="c6ad9-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="c6ad9-162">keyCredentials</span></span>|<span data-ttu-id="c6ad9-163">Коллекция [keyCredential](../resources/keycredential.md)</span><span class="sxs-lookup"><span data-stu-id="c6ad9-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="c6ad9-164">Коллекция ключевых учетных данных, связанных с субъектом-службой.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-164">The collection of key credentials associated with the service principal.</span></span> <span data-ttu-id="c6ad9-165">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-165">Not nullable.</span></span>            |
|<span data-ttu-id="c6ad9-166">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="c6ad9-166">logoutUrl</span></span>|<span data-ttu-id="c6ad9-167">String</span><span class="sxs-lookup"><span data-stu-id="c6ad9-167">String</span></span>| <span data-ttu-id="c6ad9-168">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-168">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="c6ad9-169">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="c6ad9-169">oauth2PermissionScopes</span></span>|<span data-ttu-id="c6ad9-170">Коллекция [permissionScope](../resources/permissionScope.md)</span><span class="sxs-lookup"><span data-stu-id="c6ad9-170">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="c6ad9-171">Области разрешений OAuth 2.0, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-171">The OAuth 2.0 permission scopes exposed by the associated application.</span></span> <span data-ttu-id="c6ad9-172">Дополнительные сведения см. в определении свойства **oauth2PermissionScopes** для ресурса [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="c6ad9-172">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="c6ad9-173">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-173">Not nullable.</span></span>|
|<span data-ttu-id="c6ad9-174">preferredSingleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="c6ad9-174">preferredSingleSignOnMode</span></span>|<span data-ttu-id="c6ad9-175">Строка</span><span class="sxs-lookup"><span data-stu-id="c6ad9-175">string</span></span>|<span data-ttu-id="c6ad9-176">Указывает режим единого входа, настроенный для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-176">Specifies the single sign-on mode configured for this application.</span></span> <span data-ttu-id="c6ad9-177">Azure AD использует предпочитаемый режим единого входа для запуска этого приложения из Microsoft 365 или из раздела "Мои приложения" Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-177">Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps.</span></span> <span data-ttu-id="c6ad9-178">Поддерживаемые значения: `password`, `saml`, `external` и `oidc`.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-178">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|
|<span data-ttu-id="c6ad9-179">replyUrls</span><span class="sxs-lookup"><span data-stu-id="c6ad9-179">replyUrls</span></span>|<span data-ttu-id="c6ad9-180">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c6ad9-180">String collection</span></span>|<span data-ttu-id="c6ad9-181">URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-181">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span> <span data-ttu-id="c6ad9-182">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-182">Not nullable.</span></span> |
|<span data-ttu-id="c6ad9-183">ServicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="c6ad9-183">servicePrincipalNames</span></span>|<span data-ttu-id="c6ad9-184">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c6ad9-184">String collection</span></span>|<span data-ttu-id="c6ad9-185">Содержит список объектов **identifiersUris**, скопированных из связанного объекта [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="c6ad9-185">Contains the list of **identifiersUris**, copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="c6ad9-186">К гибридным приложениям можно добавить дополнительные значения.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-186">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="c6ad9-187">С помощью этих значений можно идентифицировать разрешения, предоставленные этим приложением в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-187">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="c6ad9-188">Пример.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-188">For example,</span></span><ul><li><span data-ttu-id="c6ad9-189">Клиентские приложения, запрашивающие разрешения на доступ к этому ресурсу, могут использовать эти URI для указания необходимых разрешений в свойстве **requiredResourceAccess** манифеста приложения или в колонке "Разрешения API" в интерфейсе регистрации приложений.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-189">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="c6ad9-190">Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства, чтобы получать маркер доступа, который представляет собой URI, возвращенный в запросе "aud".</span><span class="sxs-lookup"><span data-stu-id="c6ad9-190">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="c6ad9-191">Оператор "any" требуется для выражений фильтров, применяемых к многозначным свойствам.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-191">The any operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="c6ad9-192">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-192">Not nullable.</span></span>|
|<span data-ttu-id="c6ad9-193">tags</span><span class="sxs-lookup"><span data-stu-id="c6ad9-193">tags</span></span>|<span data-ttu-id="c6ad9-194">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c6ad9-194">String collection</span></span>| <span data-ttu-id="c6ad9-195">Настраиваемые строки, которые можно использовать для классификации и определения приложения.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-195">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="c6ad9-196">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-196">Not nullable.</span></span> |
| <span data-ttu-id="c6ad9-197">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="c6ad9-197">tokenEncryptionKeyId</span></span> |<span data-ttu-id="c6ad9-198">String</span><span class="sxs-lookup"><span data-stu-id="c6ad9-198">String</span></span>|<span data-ttu-id="c6ad9-199">Задает значение открытого ключа keyId из коллекции keyCredentials.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-199">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="c6ad9-200">Если это свойство настроено, Azure AD выпускает маркеры для этого приложения в зашифрованном виде; шифрование производится с помощью ключа, указанного эти свойством.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-200">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="c6ad9-201">Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-201">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="c6ad9-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ad9-202">Response</span></span>

<span data-ttu-id="c6ad9-203">В случае успеха этот метод возвращает код отклика `204 No Content` и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-203">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6ad9-204">Пример</span><span class="sxs-lookup"><span data-stu-id="c6ad9-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6ad9-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6ad9-205">Request</span></span>
<span data-ttu-id="c6ad9-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-206">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c6ad9-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6ad9-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="c6ad9-208">C#</span><span class="sxs-lookup"><span data-stu-id="c6ad9-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6ad9-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6ad9-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6ad9-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6ad9-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6ad9-211">Java</span><span class="sxs-lookup"><span data-stu-id="c6ad9-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c6ad9-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ad9-212">Response</span></span>
<span data-ttu-id="c6ad9-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6ad9-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

