---
title: 'Страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 7772fb1de249c84785e5b19df03eab0b37ac4b83
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511105"
---
# <a name="page-copytosection"></a><span data-ttu-id="cfff6-103">Страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="cfff6-103">page: copyToSection</span></span>

<span data-ttu-id="cfff6-104">Пространство имен: Microsoft. Graph копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="cfff6-104">Namespace: microsoft.graph Copies a page to a specific section.</span></span>

<span data-ttu-id="cfff6-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="cfff6-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfff6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfff6-106">Permissions</span></span>
<span data-ttu-id="cfff6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfff6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfff6-109">Permission type</span></span>      | <span data-ttu-id="cfff6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfff6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfff6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfff6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfff6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfff6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfff6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfff6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfff6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfff6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="cfff6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfff6-115">Application</span></span> | <span data-ttu-id="cfff6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfff6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfff6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfff6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="cfff6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfff6-118">Request headers</span></span>
| <span data-ttu-id="cfff6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cfff6-119">Name</span></span>       | <span data-ttu-id="cfff6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cfff6-120">Type</span></span> | <span data-ttu-id="cfff6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cfff6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfff6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfff6-122">Authorization</span></span>  | <span data-ttu-id="cfff6-123">string</span><span class="sxs-lookup"><span data-stu-id="cfff6-123">string</span></span>  | <span data-ttu-id="cfff6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfff6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfff6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfff6-126">Content-Type</span></span> | <span data-ttu-id="cfff6-127">строка</span><span class="sxs-lookup"><span data-stu-id="cfff6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cfff6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfff6-128">Request body</span></span>
<span data-ttu-id="cfff6-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="cfff6-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="cfff6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="cfff6-130">Parameter</span></span>    | <span data-ttu-id="cfff6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cfff6-131">Type</span></span>   |<span data-ttu-id="cfff6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cfff6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfff6-133">groupId</span><span class="sxs-lookup"><span data-stu-id="cfff6-133">groupId</span></span>|<span data-ttu-id="cfff6-134">String</span><span class="sxs-lookup"><span data-stu-id="cfff6-134">String</span></span>|<span data-ttu-id="cfff6-135">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="cfff6-135">The id of the group to copy to.</span></span> <span data-ttu-id="cfff6-136">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="cfff6-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="cfff6-137">id</span><span class="sxs-lookup"><span data-stu-id="cfff6-137">id</span></span>|<span data-ttu-id="cfff6-138">String</span><span class="sxs-lookup"><span data-stu-id="cfff6-138">String</span></span>|<span data-ttu-id="cfff6-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfff6-139">Required.</span></span> <span data-ttu-id="cfff6-140">Идентификатор раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="cfff6-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="cfff6-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfff6-141">Response</span></span>

<span data-ttu-id="cfff6-142">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="cfff6-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="cfff6-143">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="cfff6-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="cfff6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="cfff6-144">Example</span></span>
<span data-ttu-id="cfff6-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cfff6-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cfff6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfff6-146">Request</span></span>
<span data-ttu-id="cfff6-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfff6-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfff6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfff6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cfff6-149">C#</span><span class="sxs-lookup"><span data-stu-id="cfff6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfff6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfff6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfff6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfff6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfff6-152">Java</span><span class="sxs-lookup"><span data-stu-id="cfff6-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cfff6-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfff6-153">Response</span></span>
<span data-ttu-id="cfff6-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfff6-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
