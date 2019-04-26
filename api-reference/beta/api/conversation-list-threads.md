---
title: Список цепочек
description: Получение всех цепочек в групповой беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3a33038abbcdf32178612278dc7f0f029cfdde1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326696"
---
# <a name="list-threads"></a><span data-ttu-id="ace5a-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="ace5a-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ace5a-104">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="ace5a-104">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="ace5a-105">Примечание. Вы также можете [получить все цепочки группы](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="ace5a-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ace5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ace5a-106">Permissions</span></span>
<span data-ttu-id="ace5a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace5a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ace5a-109">Permission type</span></span>      | <span data-ttu-id="ace5a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ace5a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace5a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ace5a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ace5a-112">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ace5a-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="ace5a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ace5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace5a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace5a-114">Not supported.</span></span>    |
|<span data-ttu-id="ace5a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ace5a-115">Application</span></span> | <span data-ttu-id="ace5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace5a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ace5a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ace5a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ace5a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ace5a-118">Optional query parameters</span></span>
<span data-ttu-id="ace5a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ace5a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ace5a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ace5a-120">Request headers</span></span>
| <span data-ttu-id="ace5a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ace5a-121">Header</span></span>       | <span data-ttu-id="ace5a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ace5a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ace5a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ace5a-123">Authorization</span></span>  | <span data-ttu-id="ace5a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ace5a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ace5a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ace5a-126">Request body</span></span>
<span data-ttu-id="ace5a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ace5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ace5a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ace5a-128">Response</span></span>

<span data-ttu-id="ace5a-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ace5a-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ace5a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ace5a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ace5a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ace5a-131">Request</span></span>
<span data-ttu-id="ace5a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ace5a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="ace5a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ace5a-133">Response</span></span>
<span data-ttu-id="ace5a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ace5a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
