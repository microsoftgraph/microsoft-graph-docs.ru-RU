---
title: Получение Примаричаннел
description: Получение свойства навигации команды, позволяющей получить доступ к общему каналу по умолчанию.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0c4b209a4f510db2c5a4cd84bbc8bf7064a7935f
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863903"
---
# <a name="get-primarychannel"></a><span data-ttu-id="ffdd7-103">Получение Примаричаннел</span><span class="sxs-lookup"><span data-stu-id="ffdd7-103">Get primaryChannel</span></span>

<span data-ttu-id="ffdd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffdd7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffdd7-105">Получение стандартного [канала](../resources/channel.md), **общего**для [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ffdd7-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffdd7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffdd7-106">Permissions</span></span>
<span data-ttu-id="ffdd7-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ffdd7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffdd7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffdd7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffdd7-109">Permission type</span></span>      | <span data-ttu-id="ffdd7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffdd7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffdd7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffdd7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ffdd7-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffdd7-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffdd7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffdd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffdd7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-114">Not supported.</span></span>    |
|<span data-ttu-id="ffdd7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ffdd7-115">Application</span></span> | <span data-ttu-id="ffdd7-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffdd7-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="ffdd7-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ffdd7-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ffdd7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffdd7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffdd7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffdd7-120">Optional query parameters</span></span>

<span data-ttu-id="ffdd7-121">Этот метод поддерживает `$filter` `$select` `$expand` [Параметры запроса](/graph/query-parameters) , и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffdd7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffdd7-122">Request headers</span></span>
| <span data-ttu-id="ffdd7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffdd7-123">Header</span></span>       | <span data-ttu-id="ffdd7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ffdd7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffdd7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffdd7-125">Authorization</span></span>  | <span data-ttu-id="ffdd7-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-126">Bearer {token}.</span></span> <span data-ttu-id="ffdd7-127">Required.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ffdd7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffdd7-128">Request body</span></span>
<span data-ttu-id="ffdd7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffdd7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffdd7-130">Response</span></span>

<span data-ttu-id="ffdd7-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffdd7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ffdd7-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffdd7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffdd7-133">Request</span></span>
<span data-ttu-id="ffdd7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ffdd7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffdd7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="ffdd7-136">C#</span><span class="sxs-lookup"><span data-stu-id="ffdd7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffdd7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffdd7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffdd7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffdd7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffdd7-139">Java</span><span class="sxs-lookup"><span data-stu-id="ffdd7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-primarychannel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ffdd7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffdd7-140">Response</span></span>
<span data-ttu-id="ffdd7-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-141">The following is an example of the response.</span></span> 

><span data-ttu-id="ffdd7-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ffdd7-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ffdd7-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get primaryChannel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
