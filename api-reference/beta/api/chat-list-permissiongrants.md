---
title: Список объектов permissionGrants чата
description: Получение списка объектов permissionGrants чата.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f66f1fd083560d98cccbce1f58f9e43ef9634b37
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990842"
---
# <a name="list-permissiongrants-of-a-chat"></a><span data-ttu-id="473dc-103">Список объектов permissionGrants чата</span><span class="sxs-lookup"><span data-stu-id="473dc-103">List permissionGrants of a chat</span></span>

<span data-ttu-id="473dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="473dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473dc-p101">Список всех [разрешений, предоставленных конкретному ресурсу](../resources/resourcespecificpermissiongrant.md) в [чате](../resources/chat.md). Это список приложений Azure AD, имеющих доступ к чату, а также типов доступа, которыми обладает каждое приложение.</span><span class="sxs-lookup"><span data-stu-id="473dc-p101">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [chat](../resources/chat.md). This is a list of Azure AD apps that have access to the chat along with the kind of access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="473dc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="473dc-107">Permissions</span></span>

<span data-ttu-id="473dc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="473dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="473dc-110">Permission Type</span></span>                        | <span data-ttu-id="473dc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="473dc-111">Permissions (from least to most privileged)</span></span>                                                                                                                                                        |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="473dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="473dc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="473dc-113">ResourceSpecificPermissionGrant.ReadForChat, TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="473dc-113">ResourceSpecificPermissionGrant.ReadForChat, TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span>                                    |
| <span data-ttu-id="473dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="473dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="473dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="473dc-115">Not supported.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="473dc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="473dc-116">Application</span></span>                            | <span data-ttu-id="473dc-117">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="473dc-117">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="473dc-118">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="473dc-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="473dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="473dc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="473dc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="473dc-120">Optional query parameters</span></span>

<span data-ttu-id="473dc-121">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="473dc-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="473dc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="473dc-122">Request headers</span></span>

| <span data-ttu-id="473dc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="473dc-123">Header</span></span>           | <span data-ttu-id="473dc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="473dc-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="473dc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="473dc-125">Authorization</span></span>    | <span data-ttu-id="473dc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="473dc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="473dc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="473dc-128">Request body</span></span>

<span data-ttu-id="473dc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="473dc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="473dc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="473dc-130">Response</span></span>

<span data-ttu-id="473dc-131">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="473dc-131">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="473dc-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="473dc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="473dc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="473dc-133">Request</span></span>

<span data-ttu-id="473dc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="473dc-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="473dc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="473dc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:089ac694c48647c68035aae675cf78ab@thread.v2/permissionGrants
```
# <a name="c"></a>[<span data-ttu-id="473dc-136">C#</span><span class="sxs-lookup"><span data-stu-id="473dc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="473dc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="473dc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="473dc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="473dc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="473dc-139">Java</span><span class="sxs-lookup"><span data-stu-id="473dc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="473dc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="473dc-140">Response</span></span>

<span data-ttu-id="473dc-141">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="473dc-141">The following example shows the response.</span></span>

><span data-ttu-id="473dc-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="473dc-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#permissionGrants",
   "value":[
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNDaGF0U2V0dGluZ3MuUmVhZFdyaXRlLkNoYXQjI0FwcGxpY2F0aW9u",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"ChatSettings.ReadWrite.Chat"
      },
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"TeamsAppInstallation.Read.Chat"
      },
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc1RhYi5EZWxldGUuQ2hhdCMjQXBwbGljYXRpb24=",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"TeamsTab.Delete.Chat"
      },
      {
         "id":"ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
         "clientAppId":"69024002-35ae-4574-a219-f261183580b4",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"74c92190-dc0e-485a-81c6-fdffd4aadfd8",
         "permissionType":"Application",
         "permission":"ChatSettings.Read.Chat"
      }
   ]
}
```

## <a name="see-also"></a><span data-ttu-id="473dc-143">См. также</span><span class="sxs-lookup"><span data-stu-id="473dc-143">See also</span></span>
- [<span data-ttu-id="473dc-144">Перечисление предоставленных разрешений команды</span><span class="sxs-lookup"><span data-stu-id="473dc-144">List permission grants of a team</span></span>](team-list-permissionGrants.md)
- [<span data-ttu-id="473dc-145">Перечисление предоставленных разрешений группы</span><span class="sxs-lookup"><span data-stu-id="473dc-145">List permission grants of a group</span></span>](group-list-permissionGrants.md)