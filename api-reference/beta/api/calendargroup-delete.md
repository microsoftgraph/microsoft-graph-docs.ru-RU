---
title: Удаление объекта calendarGroup
description: Удаление группы календарей, отличной от стандартной.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4611ae3a6e13af29af7344b43af7e575e1e37817
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440950"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="d8cdc-103">Удаление объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="d8cdc-103">Delete calendarGroup</span></span>

<span data-ttu-id="d8cdc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d8cdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8cdc-105">Удаление группы календарей, отличной от стандартной.</span><span class="sxs-lookup"><span data-stu-id="d8cdc-105">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8cdc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8cdc-106">Permissions</span></span>

<span data-ttu-id="d8cdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8cdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8cdc-109">Permission type</span></span>                        | <span data-ttu-id="d8cdc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8cdc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d8cdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8cdc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8cdc-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8cdc-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="d8cdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8cdc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8cdc-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8cdc-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="d8cdc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8cdc-115">Application</span></span>                            | <span data-ttu-id="d8cdc-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8cdc-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d8cdc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8cdc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8cdc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8cdc-118">Request headers</span></span>

| <span data-ttu-id="d8cdc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d8cdc-119">Name</span></span>          | <span data-ttu-id="d8cdc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d8cdc-120">Type</span></span>   | <span data-ttu-id="d8cdc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8cdc-121">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d8cdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8cdc-122">Authorization</span></span> | <span data-ttu-id="d8cdc-123">string</span><span class="sxs-lookup"><span data-stu-id="d8cdc-123">string</span></span> | <span data-ttu-id="d8cdc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8cdc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8cdc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8cdc-126">Request body</span></span>

<span data-ttu-id="d8cdc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8cdc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8cdc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8cdc-128">Response</span></span>

<span data-ttu-id="d8cdc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d8cdc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8cdc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8cdc-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8cdc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8cdc-132">Request</span></span>

<span data-ttu-id="d8cdc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8cdc-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d8cdc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8cdc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="d8cdc-135">C#</span><span class="sxs-lookup"><span data-stu-id="d8cdc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8cdc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8cdc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8cdc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8cdc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8cdc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8cdc-138">Response</span></span>

<span data-ttu-id="d8cdc-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8cdc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
