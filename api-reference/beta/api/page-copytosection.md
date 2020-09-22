---
title: 'Страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 189ef82b66a972146488510a3de608c88fab4d1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040436"
---
# <a name="page-copytosection"></a><span data-ttu-id="c975c-103">Страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="c975c-103">page: copyToSection</span></span>

<span data-ttu-id="c975c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c975c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c975c-105">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="c975c-105">Copies a page to a specific section.</span></span>

<span data-ttu-id="c975c-106">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="c975c-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="c975c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c975c-107">Permissions</span></span>
<span data-ttu-id="c975c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c975c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c975c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c975c-110">Permission type</span></span>      | <span data-ttu-id="c975c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c975c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c975c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c975c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c975c-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c975c-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c975c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c975c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c975c-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c975c-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c975c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c975c-116">Application</span></span> | <span data-ttu-id="c975c-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c975c-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c975c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c975c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="c975c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c975c-119">Request headers</span></span>
| <span data-ttu-id="c975c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c975c-120">Name</span></span>       | <span data-ttu-id="c975c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c975c-121">Type</span></span> | <span data-ttu-id="c975c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c975c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c975c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c975c-123">Authorization</span></span>  | <span data-ttu-id="c975c-124">string</span><span class="sxs-lookup"><span data-stu-id="c975c-124">string</span></span>  | <span data-ttu-id="c975c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c975c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c975c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c975c-127">Content-Type</span></span> | <span data-ttu-id="c975c-128">string</span><span class="sxs-lookup"><span data-stu-id="c975c-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c975c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c975c-129">Request body</span></span>
<span data-ttu-id="c975c-130">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="c975c-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="c975c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c975c-131">Parameter</span></span>    | <span data-ttu-id="c975c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c975c-132">Type</span></span>   |<span data-ttu-id="c975c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c975c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c975c-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="c975c-134">siteCollectionId</span></span>|<span data-ttu-id="c975c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="c975c-135">String</span></span>|<span data-ttu-id="c975c-136">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="c975c-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="c975c-137">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c975c-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="c975c-138">siteId</span><span class="sxs-lookup"><span data-stu-id="c975c-138">siteId</span></span>|<span data-ttu-id="c975c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="c975c-139">String</span></span>|<span data-ttu-id="c975c-140">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="c975c-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="c975c-141">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c975c-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="c975c-142">groupId</span><span class="sxs-lookup"><span data-stu-id="c975c-142">groupId</span></span>|<span data-ttu-id="c975c-143">String</span><span class="sxs-lookup"><span data-stu-id="c975c-143">String</span></span>|<span data-ttu-id="c975c-144">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="c975c-144">The id of the group to copy to.</span></span> <span data-ttu-id="c975c-145">Используйте только при копировании в группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c975c-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="c975c-146">id</span><span class="sxs-lookup"><span data-stu-id="c975c-146">id</span></span>|<span data-ttu-id="c975c-147">String</span><span class="sxs-lookup"><span data-stu-id="c975c-147">String</span></span>|<span data-ttu-id="c975c-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c975c-148">Required.</span></span> <span data-ttu-id="c975c-149">Идентификатор раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="c975c-149">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="c975c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c975c-150">Response</span></span>

<span data-ttu-id="c975c-151">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и `Operation-Location` заголовок.</span><span class="sxs-lookup"><span data-stu-id="c975c-151">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="c975c-152">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="c975c-152">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="c975c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="c975c-153">Example</span></span>
<span data-ttu-id="c975c-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c975c-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c975c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c975c-155">Request</span></span>
<span data-ttu-id="c975c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c975c-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c975c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c975c-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c975c-158">C#</span><span class="sxs-lookup"><span data-stu-id="c975c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c975c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c975c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c975c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c975c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c975c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c975c-161">Response</span></span>
<span data-ttu-id="c975c-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c975c-162">Here is an example of the response.</span></span>
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


