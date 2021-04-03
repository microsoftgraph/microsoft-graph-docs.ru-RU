---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
doc_type: apiPageType
ms.prod: microsoft-teams
localization_priority: Normal
ms.openlocfilehash: 13309e8a52be84516d8bf8c7fd5e82a51eb9330b
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507058"
---
# <a name="get-channel"></a><span data-ttu-id="9de59-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="9de59-103">Get channel</span></span>

<span data-ttu-id="9de59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9de59-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9de59-105">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9de59-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9de59-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9de59-106">Permissions</span></span>

<span data-ttu-id="9de59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9de59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de59-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9de59-109">Permission type</span></span>      | <span data-ttu-id="9de59-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9de59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9de59-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9de59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9de59-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de59-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9de59-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9de59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9de59-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9de59-114">Not supported.</span></span>    |
|<span data-ttu-id="9de59-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9de59-115">Application</span></span> | <span data-ttu-id="9de59-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de59-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="9de59-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="9de59-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="9de59-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9de59-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9de59-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="9de59-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9de59-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9de59-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9de59-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9de59-121">Optional query parameters</span></span>

<span data-ttu-id="9de59-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9de59-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9de59-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9de59-123">Request headers</span></span>

| <span data-ttu-id="9de59-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9de59-124">Header</span></span>       | <span data-ttu-id="9de59-125">Значение</span><span class="sxs-lookup"><span data-stu-id="9de59-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9de59-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9de59-126">Authorization</span></span>  | <span data-ttu-id="9de59-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9de59-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9de59-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9de59-129">Request body</span></span>

<span data-ttu-id="9de59-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9de59-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9de59-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9de59-131">Response</span></span>

<span data-ttu-id="9de59-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9de59-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de59-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9de59-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9de59-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9de59-134">Request</span></span>

<span data-ttu-id="9de59-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9de59-135">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="9de59-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9de59-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```
# <a name="c"></a>[<span data-ttu-id="9de59-137">C#</span><span class="sxs-lookup"><span data-stu-id="9de59-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9de59-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9de59-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9de59-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9de59-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9de59-140">Java</span><span class="sxs-lookup"><span data-stu-id="9de59-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9de59-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9de59-141">Response</span></span>

<span data-ttu-id="9de59-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9de59-142">Here is an example of the response.</span></span>

><span data-ttu-id="9de59-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9de59-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
    "createdDateTime": "2020-05-27T19:22:25.692Z",
    "displayName": "General",
    "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
    "membershipType": "standard"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
