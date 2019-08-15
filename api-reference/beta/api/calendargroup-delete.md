---
title: Удаление объекта calendarGroup
description: Удаление группы календарей, отличной от стандартной.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f3be2b83519a81b89abb9ed60befdf2211df24c2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419092"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="fd2f7-103">Удаление объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="fd2f7-103">Delete calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd2f7-104">Удаление группы календарей, отличной от стандартной.</span><span class="sxs-lookup"><span data-stu-id="fd2f7-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd2f7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd2f7-105">Permissions</span></span>

<span data-ttu-id="fd2f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd2f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd2f7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd2f7-108">Permission type</span></span>                        | <span data-ttu-id="fd2f7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd2f7-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fd2f7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd2f7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd2f7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd2f7-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="fd2f7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd2f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd2f7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd2f7-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="fd2f7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd2f7-114">Application</span></span>                            | <span data-ttu-id="fd2f7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd2f7-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fd2f7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd2f7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fd2f7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd2f7-117">Request headers</span></span>

| <span data-ttu-id="fd2f7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fd2f7-118">Name</span></span>          | <span data-ttu-id="fd2f7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fd2f7-119">Type</span></span>   | <span data-ttu-id="fd2f7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fd2f7-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="fd2f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd2f7-121">Authorization</span></span> | <span data-ttu-id="fd2f7-122">string</span><span class="sxs-lookup"><span data-stu-id="fd2f7-122">string</span></span> | <span data-ttu-id="fd2f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd2f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd2f7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd2f7-125">Request body</span></span>

<span data-ttu-id="fd2f7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd2f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd2f7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd2f7-127">Response</span></span>

<span data-ttu-id="fd2f7-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fd2f7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd2f7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fd2f7-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fd2f7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd2f7-131">Request</span></span>

<span data-ttu-id="fd2f7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd2f7-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fd2f7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd2f7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd2f7-134">C#</span><span class="sxs-lookup"><span data-stu-id="fd2f7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd2f7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd2f7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd2f7-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fd2f7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fd2f7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd2f7-137">Response</span></span>

<span data-ttu-id="fd2f7-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd2f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
