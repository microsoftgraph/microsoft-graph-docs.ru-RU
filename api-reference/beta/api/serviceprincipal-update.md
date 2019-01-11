---
title: Обновление serviceprincipal
description: Обновление свойства объекта serviceprincipal.
localization_priority: Normal
ms.openlocfilehash: a8d4eebe64ac9c0c658ae9c43e2e92045be67424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813029"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="ba8ba-103">Обновление serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="ba8ba-103">Update serviceprincipal</span></span>

> <span data-ttu-id="ba8ba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba8ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba8ba-106">Обновление свойства объекта serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-106">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba8ba-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8ba-107">Permissions</span></span>
<span data-ttu-id="ba8ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba8ba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8ba-110">Permission type</span></span>      | <span data-ttu-id="ba8ba-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba8ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba8ba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba8ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba8ba-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba8ba-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba8ba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba8ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba8ba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-115">Not supported.</span></span>    |
|<span data-ttu-id="ba8ba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba8ba-116">Application</span></span> | <span data-ttu-id="ba8ba-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8ba-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba8ba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba8ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ba8ba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba8ba-119">Request headers</span></span>
| <span data-ttu-id="ba8ba-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ba8ba-120">Name</span></span>       | <span data-ttu-id="ba8ba-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ba8ba-121">Type</span></span> | <span data-ttu-id="ba8ba-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ba8ba-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba8ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8ba-123">Authorization</span></span>  | <span data-ttu-id="ba8ba-124">string</span><span class="sxs-lookup"><span data-stu-id="ba8ba-124">string</span></span>  | <span data-ttu-id="ba8ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba8ba-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba8ba-127">Request body</span></span>
<span data-ttu-id="ba8ba-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ba8ba-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba8ba-131">Property</span></span>     | <span data-ttu-id="ba8ba-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ba8ba-132">Type</span></span>   |<span data-ttu-id="ba8ba-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ba8ba-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba8ba-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="ba8ba-134">accountEnabled</span></span>|<span data-ttu-id="ba8ba-135">Логический</span><span class="sxs-lookup"><span data-stu-id="ba8ba-135">Boolean</span></span>|                <span data-ttu-id="ba8ba-136">**значение true,** Если включена участника учетной записи службы. в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-136">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="ba8ba-137">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba8ba-137">appDisplayName</span></span>|<span data-ttu-id="ba8ba-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-138">String</span></span>|<span data-ttu-id="ba8ba-139">Отображаемое имя, предоставляемые элементом соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-139">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="ba8ba-140">appId</span><span class="sxs-lookup"><span data-stu-id="ba8ba-140">appId</span></span>|<span data-ttu-id="ba8ba-141">String</span><span class="sxs-lookup"><span data-stu-id="ba8ba-141">String</span></span>|<span data-ttu-id="ba8ba-142">Уникальный идентификатор для соответствующего приложения (его свойство **appId** ).</span><span class="sxs-lookup"><span data-stu-id="ba8ba-142">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="ba8ba-143">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="ba8ba-143">appRoleAssignmentRequired</span></span>|<span data-ttu-id="ba8ba-144">Логический</span><span class="sxs-lookup"><span data-stu-id="ba8ba-144">Boolean</span></span>|<span data-ttu-id="ba8ba-145">Указывает, будет ли **appRoleAssignment** пользователю или группе требуется перед Azure AD выпустит пользователя или маркер доступа к приложению.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-145">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="ba8ba-146">**Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-146">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="ba8ba-147">appRoles</span><span class="sxs-lookup"><span data-stu-id="ba8ba-147">appRoles</span></span>|<span data-ttu-id="ba8ba-148">роли приложения</span><span class="sxs-lookup"><span data-stu-id="ba8ba-148">appRole</span></span>|<span data-ttu-id="ba8ba-149">Роли приложений, предоставляемые элементом соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-149">The application roles exposed by the associated application.</span></span> <span data-ttu-id="ba8ba-150">Дополнительные сведения см в определении свойств **appRoles** на сущность приложения **примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-150">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="ba8ba-151">displayName</span><span class="sxs-lookup"><span data-stu-id="ba8ba-151">displayName</span></span>|<span data-ttu-id="ba8ba-152">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-152">String</span></span>|<span data-ttu-id="ba8ba-153">Отображаемое имя участника-службы.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-153">The display name for the service principal.</span></span>|
|<span data-ttu-id="ba8ba-154">errorUrl</span><span class="sxs-lookup"><span data-stu-id="ba8ba-154">errorUrl</span></span>|<span data-ttu-id="ba8ba-155">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-155">String</span></span>|            |
|<span data-ttu-id="ba8ba-156">Домашняя страница</span><span class="sxs-lookup"><span data-stu-id="ba8ba-156">homepage</span></span>|<span data-ttu-id="ba8ba-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-157">String</span></span>|<span data-ttu-id="ba8ba-158">URL-адрес домашней страницы соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-158">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="ba8ba-159">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="ba8ba-159">keyCredentials</span></span>|<span data-ttu-id="ba8ba-160">keyCredential</span><span class="sxs-lookup"><span data-stu-id="ba8ba-160">keyCredential</span></span>|<span data-ttu-id="ba8ba-161">Коллекция ключей учетные данные, связанные со службой участника.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-161">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="ba8ba-162">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-162">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ba8ba-163">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="ba8ba-163">logoutUrl</span></span>|<span data-ttu-id="ba8ba-164">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-164">String</span></span>| <span data-ttu-id="ba8ba-165">Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-165">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="ba8ba-166">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="ba8ba-166">oauth2Permissions</span></span>|<span data-ttu-id="ba8ba-167">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="ba8ba-167">oAuth2Permission</span></span>|<span data-ttu-id="ba8ba-168">Разрешения OAuth 2.0, предоставляемые элементом соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-168">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="ba8ba-169">Дополнительные сведения см в определении свойств **oauth2Permissions** на сущность приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-169">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="ba8ba-170">**Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-170">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="ba8ba-171">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="ba8ba-171">passwordCredentials</span></span>|<span data-ttu-id="ba8ba-172">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="ba8ba-172">passwordCredential</span></span>|<span data-ttu-id="ba8ba-173">Коллекция пароль учетных данных, связанных с участников-служб.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-173">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="ba8ba-174">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-174">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ba8ba-175">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="ba8ba-175">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="ba8ba-176">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-176">String</span></span>|<span data-ttu-id="ba8ba-177">Зарезервировано для внутреннего пользования.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-177">Reserved for internal use only.</span></span> <span data-ttu-id="ba8ba-178">Не записывать или в противном случае использовать это свойство.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-178">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="ba8ba-179">Могут быть удалены в будущих версиях.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-179">May be removed in future versions.</span></span>                            <span data-ttu-id="ba8ba-180">**Примечания**: требуется версия 1.5 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-180">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="ba8ba-181">publisherName</span><span class="sxs-lookup"><span data-stu-id="ba8ba-181">publisherName</span></span>|<span data-ttu-id="ba8ba-182">String</span><span class="sxs-lookup"><span data-stu-id="ba8ba-182">String</span></span>|<span data-ttu-id="ba8ba-183">Отображаемое имя клиента, в котором указаны соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-183">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="ba8ba-184">replyUrls</span><span class="sxs-lookup"><span data-stu-id="ba8ba-184">replyUrls</span></span>|<span data-ttu-id="ba8ba-185">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-185">String</span></span>|<span data-ttu-id="ba8ba-186">URL-адреса, что маркеры пользователей будут отправлены для входа с ним приложении или перенаправления коды авторизации коды URI, OAuth 2.0, и будут отправлены маркеры доступа для соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-186">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="ba8ba-187">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-187">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ba8ba-188">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="ba8ba-188">samlMetadataUrl</span></span>|<span data-ttu-id="ba8ba-189">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-189">String</span></span>|            |
|<span data-ttu-id="ba8ba-190">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="ba8ba-190">servicePrincipalNames</span></span>|<span data-ttu-id="ba8ba-191">Строка</span><span class="sxs-lookup"><span data-stu-id="ba8ba-191">String</span></span>|<span data-ttu-id="ba8ba-192">Коды URI, определение соответствующего приложения.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-192">The URIs that identify the associated application.</span></span> <span data-ttu-id="ba8ba-193">Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="ba8ba-193">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="ba8ba-194">**Примечания**: не допускает значение NULL, **любой** оператор для фильтра выражений на многозначные свойства; Для получения дополнительных сведений см [поддерживается запросов, фильтров и варианты страницы результатов](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="ba8ba-194">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="ba8ba-195">теги</span><span class="sxs-lookup"><span data-stu-id="ba8ba-195">tags</span></span>|<span data-ttu-id="ba8ba-196">String</span><span class="sxs-lookup"><span data-stu-id="ba8ba-196">String</span></span>|                                        <span data-ttu-id="ba8ba-197">**Примечание.** Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-197">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="ba8ba-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba8ba-198">Response</span></span>

<span data-ttu-id="ba8ba-199">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [servicePrincipal](../resources/serviceprincipal.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-199">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba8ba-200">Пример</span><span class="sxs-lookup"><span data-stu-id="ba8ba-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba8ba-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba8ba-201">Request</span></span>
<span data-ttu-id="ba8ba-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-202">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ba8ba-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba8ba-203">Response</span></span>
<span data-ttu-id="ba8ba-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ba8ba-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
