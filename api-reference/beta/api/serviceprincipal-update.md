---
title: Обновление serviceprincipal
description: Обновление свойства объекта serviceprincipal.
localization_priority: Normal
ms.openlocfilehash: 946db869863d74a94e2e9adc04a66c8d9a50e4f5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573860"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="4eb27-103">Обновление serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="4eb27-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb27-104">Обновление свойства объекта serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="4eb27-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4eb27-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb27-105">Permissions</span></span>
<span data-ttu-id="4eb27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb27-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb27-108">Permission type</span></span>      | <span data-ttu-id="4eb27-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eb27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eb27-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eb27-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4eb27-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4eb27-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4eb27-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eb27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb27-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-113">Not supported.</span></span>    |
|<span data-ttu-id="4eb27-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eb27-114">Application</span></span> | <span data-ttu-id="4eb27-115">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb27-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eb27-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eb27-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4eb27-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eb27-117">Request headers</span></span>
| <span data-ttu-id="4eb27-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4eb27-118">Name</span></span>       | <span data-ttu-id="4eb27-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4eb27-119">Type</span></span> | <span data-ttu-id="4eb27-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4eb27-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4eb27-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eb27-121">Authorization</span></span>  | <span data-ttu-id="4eb27-122">string</span><span class="sxs-lookup"><span data-stu-id="4eb27-122">string</span></span>  | <span data-ttu-id="4eb27-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eb27-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4eb27-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eb27-125">Request body</span></span>
<span data-ttu-id="4eb27-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4eb27-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4eb27-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4eb27-129">Property</span></span>     | <span data-ttu-id="4eb27-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4eb27-130">Type</span></span>   |<span data-ttu-id="4eb27-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4eb27-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4eb27-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="4eb27-132">accountEnabled</span></span>|<span data-ttu-id="4eb27-133">Логический</span><span class="sxs-lookup"><span data-stu-id="4eb27-133">Boolean</span></span>|                <span data-ttu-id="4eb27-134">**значение true,** Если включена участника учетной записи службы. в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="4eb27-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="4eb27-135">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4eb27-135">appDisplayName</span></span>|<span data-ttu-id="4eb27-136">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-136">String</span></span>|<span data-ttu-id="4eb27-137">Отображаемое имя, предоставляемые элементом соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="4eb27-138">appId</span><span class="sxs-lookup"><span data-stu-id="4eb27-138">appId</span></span>|<span data-ttu-id="4eb27-139">String</span><span class="sxs-lookup"><span data-stu-id="4eb27-139">String</span></span>|<span data-ttu-id="4eb27-140">Уникальный идентификатор для соответствующего приложения (его свойство **appId** ).</span><span class="sxs-lookup"><span data-stu-id="4eb27-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="4eb27-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="4eb27-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="4eb27-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eb27-142">Boolean</span></span>|<span data-ttu-id="4eb27-143">Указывает, будет ли **appRoleAssignment** пользователю или группе требуется перед Azure AD выпустит пользователя или маркер доступа к приложению.</span><span class="sxs-lookup"><span data-stu-id="4eb27-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="4eb27-144">**Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="4eb27-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="4eb27-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="4eb27-145">appRoles</span></span>| <span data-ttu-id="4eb27-146">[microsoft.graph.appRole](../resources/approle.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4eb27-146">[microsoft.graph.appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="4eb27-147">Роли приложений, предоставляемые элементом соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="4eb27-148">Дополнительные сведения см в определении свойств **appRoles** на сущность приложения **примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="4eb27-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="4eb27-149">displayName</span><span class="sxs-lookup"><span data-stu-id="4eb27-149">displayName</span></span>|<span data-ttu-id="4eb27-150">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-150">String</span></span>|<span data-ttu-id="4eb27-151">Отображаемое имя участника-службы.</span><span class="sxs-lookup"><span data-stu-id="4eb27-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="4eb27-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="4eb27-152">errorUrl</span></span>|<span data-ttu-id="4eb27-153">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-153">String</span></span>|            |
|<span data-ttu-id="4eb27-154">Домашняя страница</span><span class="sxs-lookup"><span data-stu-id="4eb27-154">homepage</span></span>|<span data-ttu-id="4eb27-155">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-155">String</span></span>|<span data-ttu-id="4eb27-156">URL-адрес домашней страницы соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="4eb27-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="4eb27-157">keyCredentials</span></span>|<span data-ttu-id="4eb27-158">microsoft.graph.keyCredential</span><span class="sxs-lookup"><span data-stu-id="4eb27-158">microsoft.graph.keyCredential</span></span>|<span data-ttu-id="4eb27-159">Коллекция ключей учетные данные, связанные со службой участника.</span><span class="sxs-lookup"><span data-stu-id="4eb27-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="4eb27-160">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4eb27-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="4eb27-161">logoutUrl</span></span>|<span data-ttu-id="4eb27-162">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-162">String</span></span>| <span data-ttu-id="4eb27-163">Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="4eb27-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="4eb27-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="4eb27-164">oauth2Permissions</span></span>|<span data-ttu-id="4eb27-165">microsoft.graph.oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="4eb27-165">microsoft.graph.oAuth2Permission</span></span>|<span data-ttu-id="4eb27-166">Разрешения OAuth 2.0, предоставляемые элементом соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="4eb27-167">Дополнительные сведения см в определении свойств **oauth2Permissions** на сущность приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="4eb27-168">**Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="4eb27-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="4eb27-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="4eb27-169">passwordCredentials</span></span>|<span data-ttu-id="4eb27-170">microsoft.graph.passwordCredential</span><span class="sxs-lookup"><span data-stu-id="4eb27-170">microsoft.graph.passwordCredential</span></span>|<span data-ttu-id="4eb27-171">Коллекция пароль учетных данных, связанных с участников-служб.</span><span class="sxs-lookup"><span data-stu-id="4eb27-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="4eb27-172">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4eb27-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="4eb27-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="4eb27-174">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-174">String</span></span>|<span data-ttu-id="4eb27-175">Зарезервировано для внутреннего пользования.</span><span class="sxs-lookup"><span data-stu-id="4eb27-175">Reserved for internal use only.</span></span> <span data-ttu-id="4eb27-176">Не записывать или в противном случае использовать это свойство.</span><span class="sxs-lookup"><span data-stu-id="4eb27-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="4eb27-177">Могут быть удалены в будущих версиях.</span><span class="sxs-lookup"><span data-stu-id="4eb27-177">May be removed in future versions.</span></span>                            <span data-ttu-id="4eb27-178">**Примечания**: требуется версия 1.5 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="4eb27-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="4eb27-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="4eb27-179">publisherName</span></span>|<span data-ttu-id="4eb27-180">String</span><span class="sxs-lookup"><span data-stu-id="4eb27-180">String</span></span>|<span data-ttu-id="4eb27-181">Отображаемое имя клиента, в котором указаны соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="4eb27-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="4eb27-182">replyUrls</span></span>|<span data-ttu-id="4eb27-183">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-183">String</span></span>|<span data-ttu-id="4eb27-184">URL-адреса, что маркеры пользователей будут отправлены для входа с ним приложении или перенаправления коды авторизации коды URI, OAuth 2.0, и будут отправлены маркеры доступа для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="4eb27-185">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4eb27-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="4eb27-186">samlMetadataUrl</span></span>|<span data-ttu-id="4eb27-187">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-187">String</span></span>|            |
|<span data-ttu-id="4eb27-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="4eb27-188">servicePrincipalNames</span></span>|<span data-ttu-id="4eb27-189">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-189">String</span></span>|<span data-ttu-id="4eb27-190">Коды URI, определение соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="4eb27-191">Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="4eb27-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="4eb27-192">**Примечания**: не допускает значение NULL, **любой** оператор для фильтра выражений на многозначные свойства; Для получения дополнительных сведений см [поддерживается запросов, фильтров и варианты страницы результатов](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="4eb27-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="4eb27-193">tags</span><span class="sxs-lookup"><span data-stu-id="4eb27-193">tags</span></span>|<span data-ttu-id="4eb27-194">String</span><span class="sxs-lookup"><span data-stu-id="4eb27-194">String</span></span>|                                        <span data-ttu-id="4eb27-195">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="4eb27-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb27-196">Response</span></span>

<span data-ttu-id="4eb27-197">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [servicePrincipal](../resources/serviceprincipal.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4eb27-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4eb27-198">Пример</span><span class="sxs-lookup"><span data-stu-id="4eb27-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eb27-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eb27-199">Request</span></span>
<span data-ttu-id="4eb27-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eb27-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4eb27-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb27-201">Response</span></span>
<span data-ttu-id="4eb27-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4eb27-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
