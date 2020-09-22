---
title: 'раздел: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 73bc2ed1c8a94f4f3c4d1135c929d94d6990f40f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074141"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="1d8aa-103">раздел: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="1d8aa-103">section: copyToNotebook</span></span>

<span data-ttu-id="1d8aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d8aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d8aa-105">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-105">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="1d8aa-106">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d8aa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d8aa-107">Permissions</span></span>
<span data-ttu-id="1d8aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d8aa-110">Permission type</span></span>      | <span data-ttu-id="1d8aa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d8aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d8aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d8aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d8aa-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d8aa-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d8aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d8aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d8aa-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d8aa-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1d8aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d8aa-116">Application</span></span> | <span data-ttu-id="1d8aa-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d8aa-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d8aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d8aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="1d8aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d8aa-119">Request headers</span></span>
| <span data-ttu-id="1d8aa-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1d8aa-120">Name</span></span>       | <span data-ttu-id="1d8aa-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1d8aa-121">Type</span></span> | <span data-ttu-id="1d8aa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1d8aa-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d8aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d8aa-123">Authorization</span></span>  | <span data-ttu-id="1d8aa-124">string</span><span class="sxs-lookup"><span data-stu-id="1d8aa-124">string</span></span>  | <span data-ttu-id="1d8aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d8aa-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d8aa-127">Content-Type</span></span> | <span data-ttu-id="1d8aa-128">string</span><span class="sxs-lookup"><span data-stu-id="1d8aa-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1d8aa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d8aa-129">Request body</span></span>
<span data-ttu-id="1d8aa-130">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="1d8aa-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="1d8aa-131">Parameter</span></span>    | <span data-ttu-id="1d8aa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1d8aa-132">Type</span></span>   |<span data-ttu-id="1d8aa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1d8aa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d8aa-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="1d8aa-134">siteCollectionId</span></span>|<span data-ttu-id="1d8aa-135">String</span><span class="sxs-lookup"><span data-stu-id="1d8aa-135">String</span></span>|<span data-ttu-id="1d8aa-136">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="1d8aa-137">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="1d8aa-138">siteId</span><span class="sxs-lookup"><span data-stu-id="1d8aa-138">siteId</span></span>|<span data-ttu-id="1d8aa-139">String</span><span class="sxs-lookup"><span data-stu-id="1d8aa-139">String</span></span>|<span data-ttu-id="1d8aa-140">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="1d8aa-141">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="1d8aa-142">groupId</span><span class="sxs-lookup"><span data-stu-id="1d8aa-142">groupId</span></span>|<span data-ttu-id="1d8aa-143">String</span><span class="sxs-lookup"><span data-stu-id="1d8aa-143">String</span></span>|<span data-ttu-id="1d8aa-144">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-144">The id of the group to copy to.</span></span> <span data-ttu-id="1d8aa-145">Используйте только при копировании в группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="1d8aa-146">id</span><span class="sxs-lookup"><span data-stu-id="1d8aa-146">id</span></span>|<span data-ttu-id="1d8aa-147">String</span><span class="sxs-lookup"><span data-stu-id="1d8aa-147">String</span></span>|<span data-ttu-id="1d8aa-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-148">Required.</span></span> <span data-ttu-id="1d8aa-149">Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-149">The id of the destination notebook.</span></span> |
|<span data-ttu-id="1d8aa-150">ренамеас</span><span class="sxs-lookup"><span data-stu-id="1d8aa-150">renameAs</span></span>|<span data-ttu-id="1d8aa-151">String</span><span class="sxs-lookup"><span data-stu-id="1d8aa-151">String</span></span>|<span data-ttu-id="1d8aa-152">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-152">The name of the copy.</span></span> <span data-ttu-id="1d8aa-153">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-153">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="1d8aa-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d8aa-154">Response</span></span>

<span data-ttu-id="1d8aa-155">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и `Operation-Location` заголовок.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="1d8aa-156">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="1d8aa-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="1d8aa-157">Пример</span><span class="sxs-lookup"><span data-stu-id="1d8aa-157">Example</span></span>
<span data-ttu-id="1d8aa-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d8aa-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d8aa-159">Request</span></span>
<span data-ttu-id="1d8aa-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d8aa-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d8aa-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1d8aa-162">C#</span><span class="sxs-lookup"><span data-stu-id="1d8aa-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d8aa-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d8aa-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d8aa-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d8aa-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d8aa-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d8aa-165">Response</span></span>
<span data-ttu-id="1d8aa-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1d8aa-166">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


