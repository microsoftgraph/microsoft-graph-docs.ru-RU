---
title: Получение outlookTaskFolder
description: Получите свойства и связи указанной папки задач Outlook.
ms.openlocfilehash: a5719f1fb667ed9e13d3f32cbfd9eef7394a41c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075812"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="15e1d-103">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="15e1d-103">Get outlookTaskFolder</span></span>

> <span data-ttu-id="15e1d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15e1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15e1d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15e1d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15e1d-106">Получите свойства и связи указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="15e1d-106">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="15e1d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15e1d-107">Permissions</span></span>
<span data-ttu-id="15e1d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15e1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15e1d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15e1d-110">Permission type</span></span>      | <span data-ttu-id="15e1d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15e1d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15e1d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15e1d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15e1d-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="15e1d-113">Tasks.Read</span></span>    |
|<span data-ttu-id="15e1d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15e1d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15e1d-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="15e1d-115">Tasks.Read</span></span>    |
|<span data-ttu-id="15e1d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15e1d-116">Application</span></span> | <span data-ttu-id="15e1d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15e1d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15e1d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15e1d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15e1d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15e1d-119">Optional query parameters</span></span>
<span data-ttu-id="15e1d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15e1d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15e1d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15e1d-121">Request headers</span></span>
| <span data-ttu-id="15e1d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="15e1d-122">Name</span></span>      |<span data-ttu-id="15e1d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="15e1d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15e1d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15e1d-124">Authorization</span></span>  | <span data-ttu-id="15e1d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15e1d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15e1d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15e1d-127">Request body</span></span>
<span data-ttu-id="15e1d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15e1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15e1d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="15e1d-129">Response</span></span>

<span data-ttu-id="15e1d-130">Успешно завершена, этот метод возвращает `200 OK` объект [outlookTaskFolder](../resources/outlooktaskfolder.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15e1d-130">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15e1d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="15e1d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15e1d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="15e1d-132">Request</span></span>
<span data-ttu-id="15e1d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15e1d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAAABrJAAA=')
```
##### <a name="response"></a><span data-ttu-id="15e1d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="15e1d-134">Response</span></span>
<span data-ttu-id="15e1d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="15e1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->