---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8496383023781f796389bfbaf616bc0c64b9e97e
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843256"
---
# <a name="list-channels"></a><span data-ttu-id="990ee-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="990ee-103">List channels</span></span>

<span data-ttu-id="990ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="990ee-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="990ee-105">Получение списка [каналов](../resources/channel.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="990ee-105">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="990ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="990ee-106">Permissions</span></span>
<span data-ttu-id="990ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="990ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="990ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="990ee-109">Permission type</span></span>      | <span data-ttu-id="990ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="990ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="990ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="990ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="990ee-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="990ee-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="990ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="990ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="990ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="990ee-114">Not supported.</span></span>    |
|<span data-ttu-id="990ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="990ee-115">Application</span></span> | <span data-ttu-id="990ee-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="990ee-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="990ee-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="990ee-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="990ee-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="990ee-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="990ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="990ee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="990ee-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="990ee-120">Optional query parameters</span></span>
<span data-ttu-id="990ee-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="990ee-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="990ee-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="990ee-122">Request headers</span></span>
| <span data-ttu-id="990ee-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="990ee-123">Header</span></span>       | <span data-ttu-id="990ee-124">Значение</span><span class="sxs-lookup"><span data-stu-id="990ee-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="990ee-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="990ee-125">Authorization</span></span>  | <span data-ttu-id="990ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="990ee-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="990ee-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="990ee-128">Request body</span></span>
<span data-ttu-id="990ee-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="990ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="990ee-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="990ee-130">Response</span></span>

<span data-ttu-id="990ee-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="990ee-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="990ee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="990ee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="990ee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="990ee-133">Request</span></span>
<span data-ttu-id="990ee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="990ee-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="990ee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="990ee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="990ee-136">C#</span><span class="sxs-lookup"><span data-stu-id="990ee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="990ee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="990ee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="990ee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="990ee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="990ee-139">Java</span><span class="sxs-lookup"><span data-stu-id="990ee-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="990ee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="990ee-140">Response</span></span>
<span data-ttu-id="990ee-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="990ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
