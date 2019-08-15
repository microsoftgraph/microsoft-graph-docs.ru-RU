---
title: 'раздел: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b6fcc7a5ac9005a7400f08f3c27c4dc12572cb20
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410565"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="1643f-103">раздел: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="1643f-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1643f-104">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="1643f-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="1643f-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="1643f-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="1643f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1643f-106">Permissions</span></span>
<span data-ttu-id="1643f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1643f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1643f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1643f-109">Permission type</span></span>      | <span data-ttu-id="1643f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1643f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1643f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1643f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1643f-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1643f-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1643f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1643f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1643f-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1643f-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1643f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1643f-115">Application</span></span> | <span data-ttu-id="1643f-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1643f-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1643f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1643f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="1643f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1643f-118">Request headers</span></span>
| <span data-ttu-id="1643f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1643f-119">Name</span></span>       | <span data-ttu-id="1643f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1643f-120">Type</span></span> | <span data-ttu-id="1643f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1643f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1643f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1643f-122">Authorization</span></span>  | <span data-ttu-id="1643f-123">string</span><span class="sxs-lookup"><span data-stu-id="1643f-123">string</span></span>  | <span data-ttu-id="1643f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1643f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1643f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1643f-126">Content-Type</span></span> | <span data-ttu-id="1643f-127">строка</span><span class="sxs-lookup"><span data-stu-id="1643f-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1643f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1643f-128">Request body</span></span>
<span data-ttu-id="1643f-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="1643f-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="1643f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1643f-130">Parameter</span></span>    | <span data-ttu-id="1643f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1643f-131">Type</span></span>   |<span data-ttu-id="1643f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1643f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1643f-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="1643f-133">siteCollectionId</span></span>|<span data-ttu-id="1643f-134">String</span><span class="sxs-lookup"><span data-stu-id="1643f-134">String</span></span>|<span data-ttu-id="1643f-135">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="1643f-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="1643f-136">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="1643f-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="1643f-137">siteId</span><span class="sxs-lookup"><span data-stu-id="1643f-137">siteId</span></span>|<span data-ttu-id="1643f-138">String</span><span class="sxs-lookup"><span data-stu-id="1643f-138">String</span></span>|<span data-ttu-id="1643f-139">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="1643f-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="1643f-140">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="1643f-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="1643f-141">groupId</span><span class="sxs-lookup"><span data-stu-id="1643f-141">groupId</span></span>|<span data-ttu-id="1643f-142">String</span><span class="sxs-lookup"><span data-stu-id="1643f-142">String</span></span>|<span data-ttu-id="1643f-143">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="1643f-143">The id of the group to copy to.</span></span> <span data-ttu-id="1643f-144">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="1643f-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="1643f-145">id</span><span class="sxs-lookup"><span data-stu-id="1643f-145">id</span></span>|<span data-ttu-id="1643f-146">String</span><span class="sxs-lookup"><span data-stu-id="1643f-146">String</span></span>|<span data-ttu-id="1643f-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1643f-147">Required.</span></span> <span data-ttu-id="1643f-148">Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="1643f-148">The id of the destination notebook.</span></span> |
|<span data-ttu-id="1643f-149">ренамеас</span><span class="sxs-lookup"><span data-stu-id="1643f-149">renameAs</span></span>|<span data-ttu-id="1643f-150">String</span><span class="sxs-lookup"><span data-stu-id="1643f-150">String</span></span>|<span data-ttu-id="1643f-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="1643f-151">The name of the copy.</span></span> <span data-ttu-id="1643f-152">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="1643f-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="1643f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="1643f-153">Response</span></span>

<span data-ttu-id="1643f-154">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="1643f-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="1643f-155">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="1643f-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="1643f-156">Пример</span><span class="sxs-lookup"><span data-stu-id="1643f-156">Example</span></span>
<span data-ttu-id="1643f-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1643f-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1643f-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="1643f-158">Request</span></span>
<span data-ttu-id="1643f-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1643f-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1643f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="1643f-160">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1643f-161">C#</span><span class="sxs-lookup"><span data-stu-id="1643f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1643f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1643f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1643f-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1643f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1643f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="1643f-164">Response</span></span>
<span data-ttu-id="1643f-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1643f-165">Here is an example of the response.</span></span>
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
