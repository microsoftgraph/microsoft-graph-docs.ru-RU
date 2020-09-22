---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 41fa18b7f1f576170f4383027db2d27427dbbf95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002394"
---
# <a name="remove-educationclass"></a><span data-ttu-id="f6622-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="f6622-103">Remove educationClass</span></span>

<span data-ttu-id="f6622-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6622-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6622-105">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f6622-105">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6622-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6622-106">Permissions</span></span>
<span data-ttu-id="f6622-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6622-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6622-109">Permission type</span></span>      | <span data-ttu-id="f6622-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6622-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6622-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6622-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f6622-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6622-112">Not supported.</span></span>  |
|<span data-ttu-id="f6622-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6622-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f6622-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6622-114">Not supported.</span></span>  |
|<span data-ttu-id="f6622-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6622-115">Application</span></span> | <span data-ttu-id="f6622-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6622-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f6622-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6622-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f6622-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6622-118">Request headers</span></span>
| <span data-ttu-id="f6622-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6622-119">Header</span></span>       | <span data-ttu-id="f6622-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f6622-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6622-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6622-121">Authorization</span></span>  | <span data-ttu-id="f6622-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6622-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6622-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6622-124">Request body</span></span>
<span data-ttu-id="f6622-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6622-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f6622-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6622-126">Response</span></span>
<span data-ttu-id="f6622-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="f6622-127">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6622-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f6622-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6622-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6622-129">Request</span></span>
<span data-ttu-id="f6622-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6622-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6622-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6622-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10001/classes/11001
```
# <a name="c"></a>[<span data-ttu-id="f6622-132">C#</span><span class="sxs-lookup"><span data-stu-id="f6622-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6622-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6622-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6622-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6622-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6622-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6622-135">Response</span></span>
<span data-ttu-id="f6622-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6622-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


