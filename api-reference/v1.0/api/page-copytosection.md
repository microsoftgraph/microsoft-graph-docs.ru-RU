---
title: 'страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c9bdd57eaa929c47ed6dfe5429086e0f78760e06
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788068"
---
# <a name="page-copytosection"></a><span data-ttu-id="87856-103">страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="87856-103">page: copyToSection</span></span>

<span data-ttu-id="87856-104">Пространство имен: microsoft.graph копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="87856-104">Namespace: microsoft.graph Copies a page to a specific section.</span></span>

<span data-ttu-id="87856-105">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="87856-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="87856-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87856-106">Permissions</span></span>
<span data-ttu-id="87856-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87856-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87856-109">Permission type</span></span>      | <span data-ttu-id="87856-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87856-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87856-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87856-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87856-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87856-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="87856-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87856-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87856-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87856-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="87856-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87856-115">Application</span></span> | <span data-ttu-id="87856-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87856-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87856-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87856-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="87856-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87856-118">Request headers</span></span>
| <span data-ttu-id="87856-119">Имя</span><span class="sxs-lookup"><span data-stu-id="87856-119">Name</span></span>       | <span data-ttu-id="87856-120">Тип</span><span class="sxs-lookup"><span data-stu-id="87856-120">Type</span></span> | <span data-ttu-id="87856-121">Описание</span><span class="sxs-lookup"><span data-stu-id="87856-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87856-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87856-122">Authorization</span></span>  | <span data-ttu-id="87856-123">string</span><span class="sxs-lookup"><span data-stu-id="87856-123">string</span></span>  | <span data-ttu-id="87856-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87856-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87856-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87856-126">Content-Type</span></span> | <span data-ttu-id="87856-127">string</span><span class="sxs-lookup"><span data-stu-id="87856-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="87856-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87856-128">Request body</span></span>
<span data-ttu-id="87856-129">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="87856-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="87856-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="87856-130">Parameter</span></span>    | <span data-ttu-id="87856-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87856-131">Type</span></span>   |<span data-ttu-id="87856-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87856-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87856-133">groupId</span><span class="sxs-lookup"><span data-stu-id="87856-133">groupId</span></span>|<span data-ttu-id="87856-134">String</span><span class="sxs-lookup"><span data-stu-id="87856-134">String</span></span>|<span data-ttu-id="87856-135">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="87856-135">The id of the group to copy to.</span></span> <span data-ttu-id="87856-136">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="87856-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="87856-137">id</span><span class="sxs-lookup"><span data-stu-id="87856-137">id</span></span>|<span data-ttu-id="87856-138">String</span><span class="sxs-lookup"><span data-stu-id="87856-138">String</span></span>|<span data-ttu-id="87856-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87856-139">Required.</span></span> <span data-ttu-id="87856-140">ID раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="87856-140">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="87856-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="87856-141">Response</span></span>

<span data-ttu-id="87856-142">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="87856-142">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="87856-143">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="87856-143">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="87856-144">Пример</span><span class="sxs-lookup"><span data-stu-id="87856-144">Example</span></span>
<span data-ttu-id="87856-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="87856-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87856-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="87856-146">Request</span></span>
<span data-ttu-id="87856-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87856-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87856-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="87856-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="87856-149">C#</span><span class="sxs-lookup"><span data-stu-id="87856-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87856-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87856-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87856-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87856-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87856-152">Java</span><span class="sxs-lookup"><span data-stu-id="87856-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="87856-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="87856-153">Response</span></span>
<span data-ttu-id="87856-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="87856-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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

