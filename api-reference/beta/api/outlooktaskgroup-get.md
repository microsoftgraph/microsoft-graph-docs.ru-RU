---
title: Получение outlookTaskGroup
description: Получите свойства и связи в указанную группу задач Outlook.
ms.openlocfilehash: ca1ceaf41c7664d83cfd042a61cf98c105bfdd73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082506"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="480cb-103">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="480cb-103">Get outlookTaskGroup</span></span>

> <span data-ttu-id="480cb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="480cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="480cb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="480cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="480cb-106">Получите свойства и связи в указанную группу задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="480cb-106">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="480cb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="480cb-107">Permissions</span></span>
<span data-ttu-id="480cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="480cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="480cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="480cb-110">Permission type</span></span>      | <span data-ttu-id="480cb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="480cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="480cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="480cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="480cb-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="480cb-113">Tasks.Read</span></span>    |
|<span data-ttu-id="480cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="480cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="480cb-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="480cb-115">Tasks.Read</span></span>    |
|<span data-ttu-id="480cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="480cb-116">Application</span></span> | <span data-ttu-id="480cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="480cb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="480cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="480cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="480cb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="480cb-119">Optional query parameters</span></span>
<span data-ttu-id="480cb-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="480cb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="480cb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="480cb-121">Request headers</span></span>
| <span data-ttu-id="480cb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="480cb-122">Name</span></span>      |<span data-ttu-id="480cb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="480cb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="480cb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="480cb-124">Authorization</span></span>  | <span data-ttu-id="480cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="480cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="480cb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="480cb-127">Request body</span></span>
<span data-ttu-id="480cb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="480cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="480cb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="480cb-129">Response</span></span>

<span data-ttu-id="480cb-130">Успешно завершена, этот метод возвращает `200 OK` объект [outlookTaskGroup](../resources/outlooktaskgroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="480cb-130">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="480cb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="480cb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="480cb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="480cb-132">Request</span></span>
<span data-ttu-id="480cb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="480cb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="480cb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="480cb-134">Response</span></span>
<span data-ttu-id="480cb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="480cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->