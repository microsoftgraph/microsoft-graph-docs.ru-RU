---
title: 'раздел: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: cbec8480f8c15005be086da33048bf62265b0a89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509936"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="4fb76-103">раздел: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="4fb76-103">section: copyToNotebook</span></span>

<span data-ttu-id="4fb76-104">Пространство имен: Microsoft. Graph копирует раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="4fb76-104">Namespace: microsoft.graph Copies a section to a specific notebook.</span></span>

<span data-ttu-id="4fb76-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="4fb76-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fb76-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fb76-106">Permissions</span></span>
<span data-ttu-id="4fb76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fb76-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fb76-109">Permission type</span></span>      | <span data-ttu-id="4fb76-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fb76-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fb76-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fb76-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4fb76-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb76-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4fb76-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fb76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fb76-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fb76-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4fb76-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fb76-115">Application</span></span> | <span data-ttu-id="4fb76-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb76-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fb76-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fb76-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="4fb76-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fb76-118">Request headers</span></span>
| <span data-ttu-id="4fb76-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4fb76-119">Name</span></span>       | <span data-ttu-id="4fb76-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4fb76-120">Type</span></span> | <span data-ttu-id="4fb76-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4fb76-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4fb76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fb76-122">Authorization</span></span>  | <span data-ttu-id="4fb76-123">string</span><span class="sxs-lookup"><span data-stu-id="4fb76-123">string</span></span>  | <span data-ttu-id="4fb76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fb76-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fb76-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4fb76-126">Content-Type</span></span> | <span data-ttu-id="4fb76-127">строка</span><span class="sxs-lookup"><span data-stu-id="4fb76-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4fb76-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fb76-128">Request body</span></span>
<span data-ttu-id="4fb76-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="4fb76-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="4fb76-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="4fb76-130">Parameter</span></span>    | <span data-ttu-id="4fb76-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fb76-131">Type</span></span>   |<span data-ttu-id="4fb76-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fb76-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fb76-133">groupId</span><span class="sxs-lookup"><span data-stu-id="4fb76-133">groupId</span></span>|<span data-ttu-id="4fb76-134">String</span><span class="sxs-lookup"><span data-stu-id="4fb76-134">String</span></span>|<span data-ttu-id="4fb76-135">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="4fb76-135">The id of the group to copy to.</span></span> <span data-ttu-id="4fb76-136">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="4fb76-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4fb76-137">id</span><span class="sxs-lookup"><span data-stu-id="4fb76-137">id</span></span>|<span data-ttu-id="4fb76-138">Строка</span><span class="sxs-lookup"><span data-stu-id="4fb76-138">String</span></span>|<span data-ttu-id="4fb76-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fb76-139">Required.</span></span> <span data-ttu-id="4fb76-140">Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="4fb76-140">The id of the destination notebook.</span></span> |
|<span data-ttu-id="4fb76-141">ренамеас</span><span class="sxs-lookup"><span data-stu-id="4fb76-141">renameAs</span></span>|<span data-ttu-id="4fb76-142">Строка</span><span class="sxs-lookup"><span data-stu-id="4fb76-142">String</span></span>|<span data-ttu-id="4fb76-143">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="4fb76-143">The name of the copy.</span></span> <span data-ttu-id="4fb76-144">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="4fb76-144">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="4fb76-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fb76-145">Response</span></span>

<span data-ttu-id="4fb76-146">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="4fb76-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="4fb76-147">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="4fb76-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4fb76-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4fb76-148">Example</span></span>
<span data-ttu-id="4fb76-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4fb76-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4fb76-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fb76-150">Request</span></span>
<span data-ttu-id="4fb76-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fb76-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fb76-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fb76-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4fb76-153">C#</span><span class="sxs-lookup"><span data-stu-id="4fb76-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fb76-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fb76-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fb76-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fb76-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fb76-156">Java</span><span class="sxs-lookup"><span data-stu-id="4fb76-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4fb76-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fb76-157">Response</span></span>
<span data-ttu-id="4fb76-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4fb76-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
