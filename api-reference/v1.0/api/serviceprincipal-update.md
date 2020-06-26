---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 49f9d1f19b1c77eb2b0b4873e75ec44cb5a43422
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895967"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="c2179-103">Обновление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c2179-103">Update servicePrincipal</span></span>

<span data-ttu-id="c2179-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2179-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2179-105">Обновление свойств объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="c2179-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c2179-106">Использование PATCH для установки [**пассвордкредентиал**](../resources/passwordcredential.md) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2179-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="c2179-107">Используйте методы [аддпассворд](./serviceprincipal-addpassword.md) и [ремовепассворд](./serviceprincipal-removepassword.md) , чтобы обновить пароль для servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="c2179-107">Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2179-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2179-108">Permissions</span></span>
<span data-ttu-id="c2179-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c2179-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c2179-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2179-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2179-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2179-111">Permission type</span></span>      | <span data-ttu-id="c2179-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2179-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2179-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2179-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c2179-114">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c2179-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2179-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2179-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2179-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2179-116">Not supported.</span></span>    |
|<span data-ttu-id="c2179-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2179-117">Application</span></span> | <span data-ttu-id="c2179-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2179-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2179-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2179-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c2179-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2179-120">Request headers</span></span>
| <span data-ttu-id="c2179-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c2179-121">Name</span></span>       | <span data-ttu-id="c2179-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2179-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c2179-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2179-123">Authorization</span></span> | <span data-ttu-id="c2179-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c2179-124">Bearer {token}.</span></span> <span data-ttu-id="c2179-125">Required.</span><span class="sxs-lookup"><span data-stu-id="c2179-125">Required.</span></span>  |
| <span data-ttu-id="c2179-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2179-126">Content-Type</span></span> | <span data-ttu-id="c2179-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="c2179-127">application/json.</span></span> <span data-ttu-id="c2179-128">Required.</span><span class="sxs-lookup"><span data-stu-id="c2179-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2179-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2179-129">Request body</span></span>
<span data-ttu-id="c2179-130">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="c2179-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c2179-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="c2179-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c2179-132">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="c2179-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2179-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2179-133">Property</span></span>     | <span data-ttu-id="c2179-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c2179-134">Type</span></span> |<span data-ttu-id="c2179-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c2179-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2179-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="c2179-136">accountEnabled</span></span>|<span data-ttu-id="c2179-137">Логический</span><span class="sxs-lookup"><span data-stu-id="c2179-137">Boolean</span></span>| <span data-ttu-id="c2179-138">Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c2179-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
|<span data-ttu-id="c2179-139">addIns</span><span class="sxs-lookup"><span data-stu-id="c2179-139">addIns</span></span>| [<span data-ttu-id="c2179-140">addIn</span><span class="sxs-lookup"><span data-stu-id="c2179-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="c2179-141">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="c2179-141">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="c2179-142">Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler".</span><span class="sxs-lookup"><span data-stu-id="c2179-142">For example, applications that can render file streams [may set the addIns property](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="c2179-143">Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документа, над которым работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="c2179-143">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="c2179-144">алтернативенамес</span><span class="sxs-lookup"><span data-stu-id="c2179-144">alternativeNames</span></span>|<span data-ttu-id="c2179-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2179-145">String collection</span></span>| <span data-ttu-id="c2179-146">Используется для получения субъектов служб по подписке, идентификации группы ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).</span><span class="sxs-lookup"><span data-stu-id="c2179-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="c2179-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="c2179-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="c2179-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2179-148">Boolean</span></span>|<span data-ttu-id="c2179-149">Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения.</span><span class="sxs-lookup"><span data-stu-id="c2179-149">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span> <span data-ttu-id="c2179-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-150">Not nullable.</span></span> |
|<span data-ttu-id="c2179-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="c2179-151">appRoles</span></span>|<span data-ttu-id="c2179-152">Коллекция [appRole](../resources/approle.md)</span><span class="sxs-lookup"><span data-stu-id="c2179-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="c2179-153">Роли приложения, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="c2179-153">The application roles exposed by the associated application.</span></span> <span data-ttu-id="c2179-154">Дополнительные сведения см. в описании свойства **appRoles** ресурса [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="c2179-154">For more information see the **appRoles** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="c2179-155">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-155">Not nullable.</span></span> |
|<span data-ttu-id="c2179-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c2179-156">displayName</span></span>|<span data-ttu-id="c2179-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c2179-157">String</span></span>|<span data-ttu-id="c2179-158">Отображаемое имя для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="c2179-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="c2179-159">homepage</span><span class="sxs-lookup"><span data-stu-id="c2179-159">homepage</span></span>|<span data-ttu-id="c2179-160">String</span><span class="sxs-lookup"><span data-stu-id="c2179-160">String</span></span>|<span data-ttu-id="c2179-161">Домашняя или целевая страница приложения.</span><span class="sxs-lookup"><span data-stu-id="c2179-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="c2179-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="c2179-162">keyCredentials</span></span>|<span data-ttu-id="c2179-163">Коллекция [keyCredential](../resources/keycredential.md)</span><span class="sxs-lookup"><span data-stu-id="c2179-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="c2179-164">Коллекция ключевых учетных данных, связанных с субъектом-службой.</span><span class="sxs-lookup"><span data-stu-id="c2179-164">The collection of key credentials associated with the service principal.</span></span> <span data-ttu-id="c2179-165">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-165">Not nullable.</span></span>            |
|<span data-ttu-id="c2179-166">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="c2179-166">logoutUrl</span></span>|<span data-ttu-id="c2179-167">String</span><span class="sxs-lookup"><span data-stu-id="c2179-167">String</span></span>| <span data-ttu-id="c2179-168">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="c2179-168">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="c2179-169">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="c2179-169">oauth2PermissionScopes</span></span>|<span data-ttu-id="c2179-170">Коллекция [permissionScope](../resources/permissionScope.md)</span><span class="sxs-lookup"><span data-stu-id="c2179-170">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="c2179-171">Области разрешений OAuth 2,0, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="c2179-171">The OAuth 2.0 permission scopes exposed by the associated application.</span></span> <span data-ttu-id="c2179-172">Дополнительные сведения см. в описании свойства **oauth2PermissionScopes** ресурса [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="c2179-172">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="c2179-173">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-173">Not nullable.</span></span>|
|<span data-ttu-id="c2179-174">replyUrls</span><span class="sxs-lookup"><span data-stu-id="c2179-174">replyUrls</span></span>|<span data-ttu-id="c2179-175">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2179-175">String collection</span></span>|<span data-ttu-id="c2179-176">URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="c2179-176">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span> <span data-ttu-id="c2179-177">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-177">Not nullable.</span></span> |
|<span data-ttu-id="c2179-178">ServicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="c2179-178">servicePrincipalNames</span></span>|<span data-ttu-id="c2179-179">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2179-179">String collection</span></span>|<span data-ttu-id="c2179-180">Содержит список **идентифиерсурис**, скопированных из связанного [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="c2179-180">Contains the list of **identifiersUris**, copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="c2179-181">В гибридные приложения можно добавлять дополнительные значения.</span><span class="sxs-lookup"><span data-stu-id="c2179-181">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="c2179-182">Эти значения можно использовать для определения разрешений, предоставляемых приложением в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c2179-182">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="c2179-183">For example,</span><span class="sxs-lookup"><span data-stu-id="c2179-183">For example,</span></span><ul><li><span data-ttu-id="c2179-184">Клиентские приложения, запрашивающие разрешения для этого ресурса, могут использовать эти URI для указания необходимых разрешений в свойстве **рекуиредресаурцеакцесс** манифеста приложения или в колонке "разрешения API" в функции регистрации приложений.</span><span class="sxs-lookup"><span data-stu-id="c2179-184">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="c2179-185">Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства для получения маркера доступа, который представляет собой URI, возвращенный в утверждении "ауд".</span><span class="sxs-lookup"><span data-stu-id="c2179-185">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="c2179-186">Для выражений фильтра в случае многозначных свойств требуется оператор any.</span><span class="sxs-lookup"><span data-stu-id="c2179-186">The any operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="c2179-187">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-187">Not nullable.</span></span>|
|<span data-ttu-id="c2179-188">tags</span><span class="sxs-lookup"><span data-stu-id="c2179-188">tags</span></span>|<span data-ttu-id="c2179-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2179-189">String collection</span></span>| <span data-ttu-id="c2179-190">Настраиваемые строки, которые можно использовать для классификации и определения приложения.</span><span class="sxs-lookup"><span data-stu-id="c2179-190">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="c2179-191">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c2179-191">Not nullable.</span></span> |
| <span data-ttu-id="c2179-192">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="c2179-192">tokenEncryptionKeyId</span></span> |<span data-ttu-id="c2179-193">String</span><span class="sxs-lookup"><span data-stu-id="c2179-193">String</span></span>|<span data-ttu-id="c2179-194">Задает значение открытого ключа keyId из коллекции keyCredentials.</span><span class="sxs-lookup"><span data-stu-id="c2179-194">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="c2179-195">При настройке в Azure AD маркеры проблем для этого приложения шифруются с помощью ключа, указанного этим свойством.</span><span class="sxs-lookup"><span data-stu-id="c2179-195">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="c2179-196">Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="c2179-196">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="c2179-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2179-197">Response</span></span>

<span data-ttu-id="c2179-198">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2179-198">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2179-199">Пример</span><span class="sxs-lookup"><span data-stu-id="c2179-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2179-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2179-200">Request</span></span>
<span data-ttu-id="c2179-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2179-201">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c2179-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2179-202">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c2179-203">C#</span><span class="sxs-lookup"><span data-stu-id="c2179-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2179-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2179-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2179-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2179-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2179-206">Java</span><span class="sxs-lookup"><span data-stu-id="c2179-206">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2179-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2179-207">Response</span></span>
<span data-ttu-id="c2179-208">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c2179-208">Here is an example of the response.</span></span> <span data-ttu-id="c2179-209">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c2179-209">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c2179-210">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c2179-210">All of the properties will be returned from an actual call.</span></span>
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
