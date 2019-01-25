---
title: Получение цепочки беседы
description: Получение объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5e5f0e21c8a73e10d069b5a6a7315d7713f170ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525656"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="1b57c-103">Получение цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="1b57c-103">Get conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b57c-104">Получение объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="1b57c-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b57c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b57c-105">Permissions</span></span>
<span data-ttu-id="1b57c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b57c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b57c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b57c-108">Permission type</span></span>      | <span data-ttu-id="1b57c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b57c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b57c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b57c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b57c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b57c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b57c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b57c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b57c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b57c-113">Not supported.</span></span>    |
|<span data-ttu-id="1b57c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b57c-114">Application</span></span> | <span data-ttu-id="1b57c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b57c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b57c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b57c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b57c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b57c-117">Optional query parameters</span></span>
<span data-ttu-id="1b57c-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1b57c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b57c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b57c-119">Request headers</span></span>
| <span data-ttu-id="1b57c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b57c-120">Header</span></span>       | <span data-ttu-id="1b57c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b57c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b57c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b57c-122">Authorization</span></span>  | <span data-ttu-id="1b57c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b57c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b57c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b57c-125">Request body</span></span>
<span data-ttu-id="1b57c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b57c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b57c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b57c-127">Response</span></span>
<span data-ttu-id="1b57c-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [thread](../resources/conversationthread.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1b57c-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b57c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1b57c-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1b57c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b57c-130">Request</span></span>
<span data-ttu-id="1b57c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b57c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="1b57c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b57c-132">Response</span></span>
<span data-ttu-id="1b57c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b57c-133">The following is an example of the response.</span></span>
><span data-ttu-id="1b57c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b57c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-get-thread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
