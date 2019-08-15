---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 852ea0467779ba0dab80eb0c571f39b1cf60ed9b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410134"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="0a949-103">Обновление serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="0a949-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a949-104">Обновление свойств объекта serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="0a949-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a949-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a949-105">Permissions</span></span>
<span data-ttu-id="0a949-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a949-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a949-108">Permission type</span></span>      | <span data-ttu-id="0a949-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a949-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a949-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a949-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a949-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0a949-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0a949-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a949-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a949-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a949-113">Not supported.</span></span>    |
|<span data-ttu-id="0a949-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a949-114">Application</span></span> | <span data-ttu-id="0a949-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a949-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a949-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a949-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0a949-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a949-117">Request headers</span></span>
| <span data-ttu-id="0a949-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0a949-118">Name</span></span>       | <span data-ttu-id="0a949-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0a949-119">Type</span></span> | <span data-ttu-id="0a949-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0a949-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0a949-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a949-121">Authorization</span></span>  | <span data-ttu-id="0a949-122">string</span><span class="sxs-lookup"><span data-stu-id="0a949-122">string</span></span>  | <span data-ttu-id="0a949-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a949-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a949-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a949-125">Request body</span></span>
<span data-ttu-id="0a949-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0a949-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0a949-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a949-129">Property</span></span>     | <span data-ttu-id="0a949-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0a949-130">Type</span></span>   |<span data-ttu-id="0a949-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0a949-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a949-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="0a949-132">accountEnabled</span></span>|<span data-ttu-id="0a949-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a949-133">Boolean</span></span>|                <span data-ttu-id="0a949-134">Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="0a949-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="0a949-135">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0a949-135">appDisplayName</span></span>|<span data-ttu-id="0a949-136">String</span><span class="sxs-lookup"><span data-stu-id="0a949-136">String</span></span>|<span data-ttu-id="0a949-137">Отображаемое имя, предоставляемое связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="0a949-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="0a949-138">appId</span><span class="sxs-lookup"><span data-stu-id="0a949-138">appId</span></span>|<span data-ttu-id="0a949-139">String</span><span class="sxs-lookup"><span data-stu-id="0a949-139">String</span></span>|<span data-ttu-id="0a949-140">Уникальный идентификатор для связанного приложения (его свойство **appId**).</span><span class="sxs-lookup"><span data-stu-id="0a949-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="0a949-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="0a949-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="0a949-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a949-142">Boolean</span></span>|<span data-ttu-id="0a949-143">Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения.</span><span class="sxs-lookup"><span data-stu-id="0a949-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="0a949-144">**Примечания**: требуется версия 1,5 или более новая, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="0a949-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="0a949-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="0a949-145">appRoles</span></span>|<span data-ttu-id="0a949-146">аппроле</span><span class="sxs-lookup"><span data-stu-id="0a949-146">appRole</span></span>|<span data-ttu-id="0a949-147">Роли приложения, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="0a949-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="0a949-148">Дополнительные сведения см. в описании свойства **appRoles** для объекта Application **Notes**: требуется версия 1,5 или более новая, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="0a949-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="0a949-149">displayName</span><span class="sxs-lookup"><span data-stu-id="0a949-149">displayName</span></span>|<span data-ttu-id="0a949-150">Строка</span><span class="sxs-lookup"><span data-stu-id="0a949-150">String</span></span>|<span data-ttu-id="0a949-151">Отображаемое имя для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="0a949-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="0a949-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="0a949-152">errorUrl</span></span>|<span data-ttu-id="0a949-153">String</span><span class="sxs-lookup"><span data-stu-id="0a949-153">String</span></span>|            |
|<span data-ttu-id="0a949-154">homepage</span><span class="sxs-lookup"><span data-stu-id="0a949-154">homepage</span></span>|<span data-ttu-id="0a949-155">String</span><span class="sxs-lookup"><span data-stu-id="0a949-155">String</span></span>|<span data-ttu-id="0a949-156">URL-адрес домашней страницы связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="0a949-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="0a949-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="0a949-157">keyCredentials</span></span>|<span data-ttu-id="0a949-158">кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="0a949-158">keyCredential</span></span>|<span data-ttu-id="0a949-159">Коллекция ключевых учетных данных, связанных с субъектом-службой.</span><span class="sxs-lookup"><span data-stu-id="0a949-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="0a949-160">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a949-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="0a949-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="0a949-161">logoutUrl</span></span>|<span data-ttu-id="0a949-162">String</span><span class="sxs-lookup"><span data-stu-id="0a949-162">String</span></span>| <span data-ttu-id="0a949-163">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="0a949-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="0a949-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="0a949-164">oauth2Permissions</span></span>|<span data-ttu-id="0a949-165">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="0a949-165">oAuth2Permission</span></span>|<span data-ttu-id="0a949-166">Разрешения OAuth 2.0, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="0a949-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="0a949-167">Дополнительные сведения см. в определении свойства **oauth2Permissions** для объекта application.</span><span class="sxs-lookup"><span data-stu-id="0a949-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="0a949-168">**Примечания**: требуется версия 1,5 или более новая, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="0a949-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="0a949-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="0a949-169">passwordCredentials</span></span>|<span data-ttu-id="0a949-170">пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="0a949-170">passwordCredential</span></span>|<span data-ttu-id="0a949-171">Коллекция учетных данных паролей, связанных с субъектом-службой.</span><span class="sxs-lookup"><span data-stu-id="0a949-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="0a949-172">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a949-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="0a949-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="0a949-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="0a949-174">String</span><span class="sxs-lookup"><span data-stu-id="0a949-174">String</span></span>|<span data-ttu-id="0a949-175">Зарезервировано только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="0a949-175">Reserved for internal use only.</span></span> <span data-ttu-id="0a949-176">Не записывайте и не используйте иным образом это свойство.</span><span class="sxs-lookup"><span data-stu-id="0a949-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="0a949-177">Может быть удалено в будущих версиях.</span><span class="sxs-lookup"><span data-stu-id="0a949-177">May be removed in future versions.</span></span>                            <span data-ttu-id="0a949-178">**Примечания**: требуется версия 1,5 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="0a949-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="0a949-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="0a949-179">publisherName</span></span>|<span data-ttu-id="0a949-180">String</span><span class="sxs-lookup"><span data-stu-id="0a949-180">String</span></span>|<span data-ttu-id="0a949-181">Отображаемое имя клиента, в котором указано связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="0a949-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="0a949-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="0a949-182">replyUrls</span></span>|<span data-ttu-id="0a949-183">String</span><span class="sxs-lookup"><span data-stu-id="0a949-183">String</span></span>|<span data-ttu-id="0a949-184">URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="0a949-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="0a949-185">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a949-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="0a949-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="0a949-186">samlMetadataUrl</span></span>|<span data-ttu-id="0a949-187">String</span><span class="sxs-lookup"><span data-stu-id="0a949-187">String</span></span>|            |
|<span data-ttu-id="0a949-188">ServicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="0a949-188">servicePrincipalNames</span></span>|<span data-ttu-id="0a949-189">String</span><span class="sxs-lookup"><span data-stu-id="0a949-189">String</span></span>|<span data-ttu-id="0a949-190">URI, определяющие связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="0a949-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="0a949-191">Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="0a949-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="0a949-192">**Notes**: not Nullable, оператор **ANY** необходим для выражений фильтров в многозначных свойствах; Дополнительные сведения см в разделе [Поддерживаемые запросы, фильтры и параметры разбиения по страницам](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="0a949-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="0a949-193">tags</span><span class="sxs-lookup"><span data-stu-id="0a949-193">tags</span></span>|<span data-ttu-id="0a949-194">String</span><span class="sxs-lookup"><span data-stu-id="0a949-194">String</span></span>|                                        <span data-ttu-id="0a949-195">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a949-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="0a949-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a949-196">Response</span></span>

<span data-ttu-id="0a949-197">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a949-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a949-198">Пример</span><span class="sxs-lookup"><span data-stu-id="0a949-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a949-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a949-199">Request</span></span>
<span data-ttu-id="0a949-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a949-200">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a949-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a949-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a949-202">C#</span><span class="sxs-lookup"><span data-stu-id="0a949-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a949-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a949-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a949-204">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0a949-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a949-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a949-205">Response</span></span>
<span data-ttu-id="0a949-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a949-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
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
