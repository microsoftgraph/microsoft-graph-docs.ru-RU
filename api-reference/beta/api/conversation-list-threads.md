---
title: Список цепочек
description: Получение всех цепочек в групповой беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: bdef7c4a5fe6d28772cff5ed0f286065595e1088
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519404"
---
# <a name="list-threads"></a><span data-ttu-id="fec9f-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="fec9f-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fec9f-104">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="fec9f-104">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="fec9f-105">Примечание. Вы также можете [получить все цепочки группы](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="fec9f-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="fec9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fec9f-106">Permissions</span></span>
<span data-ttu-id="fec9f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fec9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fec9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fec9f-109">Permission type</span></span>      | <span data-ttu-id="fec9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fec9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fec9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fec9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fec9f-112">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fec9f-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="fec9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fec9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fec9f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fec9f-114">Not supported.</span></span>    |
|<span data-ttu-id="fec9f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fec9f-115">Application</span></span> | <span data-ttu-id="fec9f-116">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fec9f-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fec9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fec9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fec9f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fec9f-118">Optional query parameters</span></span>
<span data-ttu-id="fec9f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fec9f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fec9f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fec9f-120">Request headers</span></span>
| <span data-ttu-id="fec9f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fec9f-121">Header</span></span>       | <span data-ttu-id="fec9f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fec9f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fec9f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fec9f-123">Authorization</span></span>  | <span data-ttu-id="fec9f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fec9f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fec9f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fec9f-126">Request body</span></span>
<span data-ttu-id="fec9f-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fec9f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fec9f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fec9f-128">Response</span></span>

<span data-ttu-id="fec9f-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fec9f-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fec9f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fec9f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fec9f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fec9f-131">Request</span></span>
<span data-ttu-id="fec9f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fec9f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="fec9f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="fec9f-133">Response</span></span>
<span data-ttu-id="fec9f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fec9f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversation-list-threads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
