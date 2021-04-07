---
title: Список объектов permissionGrants группы
description: Получение списка объектов permissionGrants группы.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 64d3eaf0fde0dc6e822dbb0bfaa3a52daab680f4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611366"
---
# <a name="list-permissiongrants-of-a-group"></a><span data-ttu-id="c8690-103">Список объектов permissionGrants группы</span><span class="sxs-lookup"><span data-stu-id="c8690-103">List permissionGrants of a group</span></span>

<span data-ttu-id="c8690-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8690-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8690-105">Список всех [разрешений, предоставленных конкретному ресурсу](../resources/resourcespecificpermissiongrant.md) в [группе](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="c8690-105">List all [resource-specific permission grants](../resources/resourcespecificpermissiongrant.md) on the [group](../resources/group.md).</span></span> <span data-ttu-id="c8690-106">Это список приложений Azure AD, имеющих доступ к чату, одновременно с доступом, который имеет каждое приложение.</span><span class="sxs-lookup"><span data-stu-id="c8690-106">This is a list of Azure AD apps that have access to the chat along with the kind of access that each app has.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8690-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8690-107">Permissions</span></span>

<span data-ttu-id="c8690-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8690-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8690-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8690-110">Permission Type</span></span>                        | <span data-ttu-id="c8690-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8690-111">Permissions (from least to most privileged)</span></span>                                          |
| :------------------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="c8690-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8690-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8690-113">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8690-113">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c8690-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8690-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8690-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8690-115">Not supported.</span></span>                                                                       |
| <span data-ttu-id="c8690-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8690-116">Application</span></span>                            | <span data-ttu-id="c8690-117">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8690-117">GroupMember.Read.All, GroupMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8690-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8690-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{group-id}/permissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8690-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8690-119">Optional query parameters</span></span>

<span data-ttu-id="c8690-120">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c8690-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8690-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8690-121">Request headers</span></span>

| <span data-ttu-id="c8690-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8690-122">Header</span></span>           | <span data-ttu-id="c8690-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c8690-123">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="c8690-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8690-124">Authorization</span></span>    | <span data-ttu-id="c8690-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8690-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8690-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8690-127">Request body</span></span>

<span data-ttu-id="c8690-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8690-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8690-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8690-129">Response</span></span>

<span data-ttu-id="c8690-130">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8690-130">If successful, this method returns a `200 OK` response code and a list of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8690-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8690-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8690-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8690-132">Request</span></span>

<span data-ttu-id="c8690-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8690-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c8690-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8690-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants
```
# <a name="c"></a>[<span data-ttu-id="c8690-135">C#</span><span class="sxs-lookup"><span data-stu-id="c8690-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8690-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8690-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8690-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8690-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8690-138">Java</span><span class="sxs-lookup"><span data-stu-id="c8690-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c8690-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8690-139">Response</span></span>

<span data-ttu-id="c8690-140">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8690-140">The following example shows the response.</span></span>

><span data-ttu-id="c8690-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8690-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#permissionGrants",
    "value": [
        {
            "id": "ZfwbxSIj9OGOBxsBmwY555mOHr_W6qN7LEbFYIIcM5A",
            "deletedDateTime": null,
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        },
        {
            "id": "WsYCHhlwjliiK19ONpJiWq6rtFy-Tg1q8h9-f-DATto",
            "deletedDateTime": null,
            "clientId": "771b9da9-2260-41eb-a587-4d936e4aa08c",
            "clientAppId": "fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamsTab.Create.Group"
        },
        {
            "id": "wtAZautz7ilRA0kgHYWr2Ss2FTK3jPkf-HPhj3FS1wo",
            "deletedDateTime": null,
            "clientId": "74c92190-dc0e-485a-81c6-fdffd4aadfd8",
            "clientAppId": "69024002-35ae-4574-a219-f261183580b4",
            "resourceAppId": "00000003-0000-0000-c000-000000000000",
            "permissionType": "Application",
            "permission": "TeamMember.Read.Group"
        }
    ]
}
```
