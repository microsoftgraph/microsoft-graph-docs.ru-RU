---
title: Список вложений
description: Получение списка объектов вложений, вложенных в задачу Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d694d8b3b39502ac85c59dcef52a8bb2afb77577
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266796"
---
# <a name="list-attachments"></a><span data-ttu-id="fd348-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="fd348-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd348-104">Получение списка объектов [вложений](../resources/attachment.md) , вложенных в задачу Outlook.</span><span class="sxs-lookup"><span data-stu-id="fd348-104">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd348-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd348-105">Permissions</span></span>

<span data-ttu-id="fd348-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd348-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd348-108">Permission type</span></span>      | <span data-ttu-id="fd348-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd348-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd348-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd348-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd348-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fd348-111">Tasks.Read</span></span>    |
|<span data-ttu-id="fd348-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd348-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd348-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fd348-113">Tasks.Read</span></span>    |
|<span data-ttu-id="fd348-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd348-114">Application</span></span> | <span data-ttu-id="fd348-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd348-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd348-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd348-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd348-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd348-117">Optional query parameters</span></span>

<span data-ttu-id="fd348-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fd348-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd348-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd348-119">Request headers</span></span>

| <span data-ttu-id="fd348-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fd348-120">Name</span></span>      |<span data-ttu-id="fd348-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fd348-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd348-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd348-122">Authorization</span></span>  | <span data-ttu-id="fd348-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd348-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd348-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd348-125">Request body</span></span>

<span data-ttu-id="fd348-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd348-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd348-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd348-127">Response</span></span>

<span data-ttu-id="fd348-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вложений](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd348-128">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd348-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fd348-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd348-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd348-130">Request</span></span>

<span data-ttu-id="fd348-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd348-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="fd348-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd348-132">Response</span></span>

<span data-ttu-id="fd348-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd348-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd348-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fd348-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd348-137">C#</span><span class="sxs-lookup"><span data-stu-id="fd348-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd348-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="fd348-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fd348-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fd348-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_attachments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktask-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
