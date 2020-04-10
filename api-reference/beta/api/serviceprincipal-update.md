---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 072351ebc95d8610bc069055aacb0b193e1ca626
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218607"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="cd954-103">Обновление serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="cd954-103">Update serviceprincipal</span></span>

<span data-ttu-id="cd954-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd954-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd954-105">Обновление свойств объекта serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="cd954-105">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd954-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd954-106">Permissions</span></span>
<span data-ttu-id="cd954-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd954-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd954-109">Permission type</span></span>      | <span data-ttu-id="cd954-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd954-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd954-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd954-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd954-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd954-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd954-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd954-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd954-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd954-114">Not supported.</span></span>    |
|<span data-ttu-id="cd954-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd954-115">Application</span></span> | <span data-ttu-id="cd954-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd954-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd954-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd954-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cd954-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd954-118">Request headers</span></span>
| <span data-ttu-id="cd954-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cd954-119">Name</span></span>       | <span data-ttu-id="cd954-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cd954-120">Type</span></span> | <span data-ttu-id="cd954-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cd954-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd954-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd954-122">Authorization</span></span>  | <span data-ttu-id="cd954-123">string</span><span class="sxs-lookup"><span data-stu-id="cd954-123">string</span></span>  | <span data-ttu-id="cd954-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd954-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd954-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd954-126">Request body</span></span>
<span data-ttu-id="cd954-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cd954-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd954-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd954-130">Property</span></span>     | <span data-ttu-id="cd954-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cd954-131">Type</span></span>   |<span data-ttu-id="cd954-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cd954-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd954-133">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="cd954-133">accountEnabled</span></span>|<span data-ttu-id="cd954-134">Логический</span><span class="sxs-lookup"><span data-stu-id="cd954-134">Boolean</span></span>|                <span data-ttu-id="cd954-135">Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="cd954-135">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="cd954-136">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="cd954-136">appDisplayName</span></span>|<span data-ttu-id="cd954-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-137">String</span></span>|<span data-ttu-id="cd954-138">Отображаемое имя, предоставляемое связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="cd954-138">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="cd954-139">appId</span><span class="sxs-lookup"><span data-stu-id="cd954-139">appId</span></span>|<span data-ttu-id="cd954-140">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-140">String</span></span>|<span data-ttu-id="cd954-141">Уникальный идентификатор для связанного приложения (его свойство **appId**).</span><span class="sxs-lookup"><span data-stu-id="cd954-141">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="cd954-142">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="cd954-142">appRoleAssignmentRequired</span></span>|<span data-ttu-id="cd954-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd954-143">Boolean</span></span>|<span data-ttu-id="cd954-144">Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd954-144">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="cd954-145">**Примечания**: требуется версия 1,5 или более новая, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="cd954-145">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="cd954-146">appRoles</span><span class="sxs-lookup"><span data-stu-id="cd954-146">appRoles</span></span>|<span data-ttu-id="cd954-147">аппроле</span><span class="sxs-lookup"><span data-stu-id="cd954-147">appRole</span></span>|<span data-ttu-id="cd954-148">Роли приложения, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="cd954-148">The application roles exposed by the associated application.</span></span> <span data-ttu-id="cd954-149">Дополнительные сведения см. в описании свойства **appRoles** для объекта Application **Notes**: требуется версия 1,5 или более новая, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="cd954-149">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="cd954-150">displayName</span><span class="sxs-lookup"><span data-stu-id="cd954-150">displayName</span></span>|<span data-ttu-id="cd954-151">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-151">String</span></span>|<span data-ttu-id="cd954-152">Отображаемое имя для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cd954-152">The display name for the service principal.</span></span>|
|<span data-ttu-id="cd954-153">errorUrl</span><span class="sxs-lookup"><span data-stu-id="cd954-153">errorUrl</span></span>|<span data-ttu-id="cd954-154">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-154">String</span></span>|            |
|<span data-ttu-id="cd954-155">homepage</span><span class="sxs-lookup"><span data-stu-id="cd954-155">homepage</span></span>|<span data-ttu-id="cd954-156">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-156">String</span></span>|<span data-ttu-id="cd954-157">URL-адрес домашней страницы связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="cd954-157">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="cd954-158">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="cd954-158">keyCredentials</span></span>|<span data-ttu-id="cd954-159">кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="cd954-159">keyCredential</span></span>|<span data-ttu-id="cd954-160">Коллекция ключевых учетных данных, связанных с субъектом-службой.</span><span class="sxs-lookup"><span data-stu-id="cd954-160">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="cd954-161">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cd954-161">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cd954-162">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="cd954-162">logoutUrl</span></span>|<span data-ttu-id="cd954-163">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-163">String</span></span>| <span data-ttu-id="cd954-164">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="cd954-164">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="cd954-165">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="cd954-165">oauth2Permissions</span></span>|<span data-ttu-id="cd954-166">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="cd954-166">oAuth2Permission</span></span>|<span data-ttu-id="cd954-167">Разрешения OAuth 2.0, предоставляемые связанным приложением.</span><span class="sxs-lookup"><span data-stu-id="cd954-167">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="cd954-168">Дополнительные сведения см. в определении свойства **oauth2Permissions** для объекта application.</span><span class="sxs-lookup"><span data-stu-id="cd954-168">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="cd954-169">**Примечания**: требуется версия 1,5 или более новая, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="cd954-169">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="cd954-170">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="cd954-170">passwordCredentials</span></span>|<span data-ttu-id="cd954-171">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="cd954-171">passwordCredential</span></span>|<span data-ttu-id="cd954-172">Коллекция учетных данных паролей, связанных с субъектом-службой.</span><span class="sxs-lookup"><span data-stu-id="cd954-172">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="cd954-173">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cd954-173">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cd954-174">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="cd954-174">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="cd954-175">String</span><span class="sxs-lookup"><span data-stu-id="cd954-175">String</span></span>|<span data-ttu-id="cd954-176">Зарезервировано только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="cd954-176">Reserved for internal use only.</span></span> <span data-ttu-id="cd954-177">Не записывайте и не используйте иным образом это свойство.</span><span class="sxs-lookup"><span data-stu-id="cd954-177">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="cd954-178">Может быть удалено в будущих версиях.</span><span class="sxs-lookup"><span data-stu-id="cd954-178">May be removed in future versions.</span></span>                            <span data-ttu-id="cd954-179">**Примечания**: требуется версия 1,5 или более поздняя.</span><span class="sxs-lookup"><span data-stu-id="cd954-179">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="cd954-180">publisherName</span><span class="sxs-lookup"><span data-stu-id="cd954-180">publisherName</span></span>|<span data-ttu-id="cd954-181">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-181">String</span></span>|<span data-ttu-id="cd954-182">Отображаемое имя клиента, в котором указано связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="cd954-182">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="cd954-183">replyUrls</span><span class="sxs-lookup"><span data-stu-id="cd954-183">replyUrls</span></span>|<span data-ttu-id="cd954-184">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-184">String</span></span>|<span data-ttu-id="cd954-185">URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения.</span><span class="sxs-lookup"><span data-stu-id="cd954-185">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="cd954-186">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cd954-186">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cd954-187">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="cd954-187">samlMetadataUrl</span></span>|<span data-ttu-id="cd954-188">String</span><span class="sxs-lookup"><span data-stu-id="cd954-188">String</span></span>|            |
|<span data-ttu-id="cd954-189">ServicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="cd954-189">servicePrincipalNames</span></span>|<span data-ttu-id="cd954-190">Строка</span><span class="sxs-lookup"><span data-stu-id="cd954-190">String</span></span>|<span data-ttu-id="cd954-191">URI, определяющие связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="cd954-191">The URIs that identify the associated application.</span></span> <span data-ttu-id="cd954-192">Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="cd954-192">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="cd954-193">**Notes**: not Nullable, оператор **ANY** необходим для выражений фильтров в многозначных свойствах; Дополнительные сведения см в разделе [Поддерживаемые запросы, фильтры и параметры разбиения по страницам](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="cd954-193">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="cd954-194">tags</span><span class="sxs-lookup"><span data-stu-id="cd954-194">tags</span></span>|<span data-ttu-id="cd954-195">String</span><span class="sxs-lookup"><span data-stu-id="cd954-195">String</span></span>|                                        <span data-ttu-id="cd954-196">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cd954-196">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="cd954-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd954-197">Response</span></span>

<span data-ttu-id="cd954-198">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd954-198">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd954-199">Пример</span><span class="sxs-lookup"><span data-stu-id="cd954-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd954-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd954-200">Request</span></span>
<span data-ttu-id="cd954-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd954-201">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd954-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd954-202">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd954-203">C#</span><span class="sxs-lookup"><span data-stu-id="cd954-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd954-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd954-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd954-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd954-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cd954-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd954-206">Response</span></span>
<span data-ttu-id="cd954-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd954-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
