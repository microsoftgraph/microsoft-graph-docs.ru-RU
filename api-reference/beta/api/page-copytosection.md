---
title: 'страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 665d244248c8af3a4ce3b5b01151d3debe196d92
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785237"
---
# <a name="page-copytosection"></a><span data-ttu-id="d6b4b-103">страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="d6b4b-103">page: copyToSection</span></span>

<span data-ttu-id="d6b4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6b4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6b4b-105">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-105">Copies a page to a specific section.</span></span>

<span data-ttu-id="d6b4b-106">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6b4b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b4b-107">Permissions</span></span>
<span data-ttu-id="d6b4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b4b-110">Permission type</span></span>      | <span data-ttu-id="d6b4b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6b4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6b4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6b4b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d6b4b-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b4b-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6b4b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6b4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6b4b-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6b4b-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d6b4b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6b4b-116">Application</span></span> | <span data-ttu-id="d6b4b-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b4b-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6b4b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6b4b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="d6b4b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6b4b-119">Request headers</span></span>
| <span data-ttu-id="d6b4b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d6b4b-120">Name</span></span>       | <span data-ttu-id="d6b4b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d6b4b-121">Type</span></span> | <span data-ttu-id="d6b4b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b4b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6b4b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b4b-123">Authorization</span></span>  | <span data-ttu-id="d6b4b-124">string</span><span class="sxs-lookup"><span data-stu-id="d6b4b-124">string</span></span>  | <span data-ttu-id="d6b4b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6b4b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6b4b-127">Content-Type</span></span> | <span data-ttu-id="d6b4b-128">string</span><span class="sxs-lookup"><span data-stu-id="d6b4b-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d6b4b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6b4b-129">Request body</span></span>
<span data-ttu-id="d6b4b-130">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="d6b4b-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="d6b4b-131">Parameter</span></span>    | <span data-ttu-id="d6b4b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d6b4b-132">Type</span></span>   |<span data-ttu-id="d6b4b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b4b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6b4b-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="d6b4b-134">siteCollectionId</span></span>|<span data-ttu-id="d6b4b-135">String</span><span class="sxs-lookup"><span data-stu-id="d6b4b-135">String</span></span>|<span data-ttu-id="d6b4b-136">ID сайта SharePoint скопировать.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="d6b4b-137">Используйте только при копировании на SharePoint сайте.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="d6b4b-138">siteId</span><span class="sxs-lookup"><span data-stu-id="d6b4b-138">siteId</span></span>|<span data-ttu-id="d6b4b-139">String</span><span class="sxs-lookup"><span data-stu-id="d6b4b-139">String</span></span>|<span data-ttu-id="d6b4b-140">ID веб-SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="d6b4b-141">Используйте только при копировании на SharePoint сайте.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="d6b4b-142">groupId</span><span class="sxs-lookup"><span data-stu-id="d6b4b-142">groupId</span></span>|<span data-ttu-id="d6b4b-143">String</span><span class="sxs-lookup"><span data-stu-id="d6b4b-143">String</span></span>|<span data-ttu-id="d6b4b-144">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-144">The id of the group to copy to.</span></span> <span data-ttu-id="d6b4b-145">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="d6b4b-146">id</span><span class="sxs-lookup"><span data-stu-id="d6b4b-146">id</span></span>|<span data-ttu-id="d6b4b-147">String</span><span class="sxs-lookup"><span data-stu-id="d6b4b-147">String</span></span>|<span data-ttu-id="d6b4b-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-148">Required.</span></span> <span data-ttu-id="d6b4b-149">ID раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-149">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="d6b4b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b4b-150">Response</span></span>

<span data-ttu-id="d6b4b-151">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-151">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="d6b4b-152">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="d6b4b-152">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d6b4b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d6b4b-153">Example</span></span>
<span data-ttu-id="d6b4b-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d6b4b-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6b4b-155">Request</span></span>
<span data-ttu-id="d6b4b-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6b4b-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6b4b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d6b4b-158">C#</span><span class="sxs-lookup"><span data-stu-id="d6b4b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6b4b-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6b4b-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6b4b-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6b4b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6b4b-161">Java</span><span class="sxs-lookup"><span data-stu-id="d6b4b-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6b4b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b4b-162">Response</span></span>
<span data-ttu-id="d6b4b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6b4b-163">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


