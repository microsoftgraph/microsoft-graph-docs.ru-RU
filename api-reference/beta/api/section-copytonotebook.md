---
title: 'раздел: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5a1d99f93df7acd6c964ae690784ab3df8cca43c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978690"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="7f710-103">раздел: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="7f710-103">section: copyToNotebook</span></span>

<span data-ttu-id="7f710-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f710-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f710-105">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="7f710-105">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="7f710-106">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="7f710-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f710-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f710-107">Permissions</span></span>
<span data-ttu-id="7f710-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f710-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f710-110">Permission type</span></span>      | <span data-ttu-id="7f710-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f710-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f710-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f710-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f710-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f710-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f710-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f710-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f710-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f710-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7f710-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f710-116">Application</span></span> | <span data-ttu-id="7f710-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f710-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f710-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f710-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="7f710-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f710-119">Request headers</span></span>
| <span data-ttu-id="7f710-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7f710-120">Name</span></span>       | <span data-ttu-id="7f710-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7f710-121">Type</span></span> | <span data-ttu-id="7f710-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7f710-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f710-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f710-123">Authorization</span></span>  | <span data-ttu-id="7f710-124">string</span><span class="sxs-lookup"><span data-stu-id="7f710-124">string</span></span>  | <span data-ttu-id="7f710-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f710-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f710-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f710-127">Content-Type</span></span> | <span data-ttu-id="7f710-128">string</span><span class="sxs-lookup"><span data-stu-id="7f710-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7f710-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f710-129">Request body</span></span>
<span data-ttu-id="7f710-130">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="7f710-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="7f710-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="7f710-131">Parameter</span></span>    | <span data-ttu-id="7f710-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7f710-132">Type</span></span>   |<span data-ttu-id="7f710-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7f710-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f710-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="7f710-134">siteCollectionId</span></span>|<span data-ttu-id="7f710-135">String</span><span class="sxs-lookup"><span data-stu-id="7f710-135">String</span></span>|<span data-ttu-id="7f710-136">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="7f710-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="7f710-137">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7f710-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="7f710-138">siteId</span><span class="sxs-lookup"><span data-stu-id="7f710-138">siteId</span></span>|<span data-ttu-id="7f710-139">String</span><span class="sxs-lookup"><span data-stu-id="7f710-139">String</span></span>|<span data-ttu-id="7f710-140">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="7f710-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="7f710-141">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7f710-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="7f710-142">groupId</span><span class="sxs-lookup"><span data-stu-id="7f710-142">groupId</span></span>|<span data-ttu-id="7f710-143">String</span><span class="sxs-lookup"><span data-stu-id="7f710-143">String</span></span>|<span data-ttu-id="7f710-144">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="7f710-144">The id of the group to copy to.</span></span> <span data-ttu-id="7f710-145">Используйте только при копировании в группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7f710-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="7f710-146">id</span><span class="sxs-lookup"><span data-stu-id="7f710-146">id</span></span>|<span data-ttu-id="7f710-147">String</span><span class="sxs-lookup"><span data-stu-id="7f710-147">String</span></span>|<span data-ttu-id="7f710-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f710-148">Required.</span></span> <span data-ttu-id="7f710-149">Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="7f710-149">The id of the destination notebook.</span></span> |
|<span data-ttu-id="7f710-150">ренамеас</span><span class="sxs-lookup"><span data-stu-id="7f710-150">renameAs</span></span>|<span data-ttu-id="7f710-151">String</span><span class="sxs-lookup"><span data-stu-id="7f710-151">String</span></span>|<span data-ttu-id="7f710-152">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="7f710-152">The name of the copy.</span></span> <span data-ttu-id="7f710-153">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="7f710-153">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="7f710-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f710-154">Response</span></span>

<span data-ttu-id="7f710-155">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и `Operation-Location` заголовок.</span><span class="sxs-lookup"><span data-stu-id="7f710-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="7f710-156">Опрос конечной точки Operation-Location для [получения состояния операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="7f710-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="7f710-157">Пример</span><span class="sxs-lookup"><span data-stu-id="7f710-157">Example</span></span>
<span data-ttu-id="7f710-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7f710-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7f710-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f710-159">Request</span></span>
<span data-ttu-id="7f710-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f710-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f710-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f710-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7f710-162">C#</span><span class="sxs-lookup"><span data-stu-id="7f710-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f710-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f710-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f710-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f710-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f710-165">Java</span><span class="sxs-lookup"><span data-stu-id="7f710-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f710-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f710-166">Response</span></span>
<span data-ttu-id="7f710-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f710-167">Here is an example of the response.</span></span>
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


