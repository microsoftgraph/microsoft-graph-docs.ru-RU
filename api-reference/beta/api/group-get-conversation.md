---
title: Получение беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 374fd472cf97e17586ea9e95c55f765c5d79dc34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892374"
---
# <a name="get-conversation"></a><span data-ttu-id="e3614-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="e3614-103">Get conversation</span></span>

> <span data-ttu-id="e3614-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3614-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3614-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3614-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3614-106">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="e3614-106">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3614-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3614-107">Permissions</span></span>
<span data-ttu-id="e3614-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3614-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3614-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3614-110">Permission type</span></span>      | <span data-ttu-id="e3614-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3614-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3614-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3614-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3614-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3614-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3614-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3614-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3614-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3614-115">Not supported.</span></span>    |
|<span data-ttu-id="e3614-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3614-116">Application</span></span> | <span data-ttu-id="e3614-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3614-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3614-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3614-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3614-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3614-119">Optional query parameters</span></span>
<span data-ttu-id="e3614-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e3614-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3614-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3614-121">Request headers</span></span>
| <span data-ttu-id="e3614-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3614-122">Header</span></span>       | <span data-ttu-id="e3614-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e3614-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3614-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3614-124">Authorization</span></span>  | <span data-ttu-id="e3614-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3614-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3614-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3614-127">Request body</span></span>
<span data-ttu-id="e3614-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3614-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3614-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3614-129">Response</span></span>
<span data-ttu-id="e3614-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3614-130">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3614-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e3614-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e3614-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3614-132">Request</span></span>
<span data-ttu-id="e3614-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3614-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="e3614-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3614-134">Response</span></span>
<span data-ttu-id="e3614-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3614-135">The following is an example of the response.</span></span>
><span data-ttu-id="e3614-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3614-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
