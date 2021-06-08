---
title: 'раздел: copyToNotebook'
description: Копирует раздел в определенный блокнот.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9b47c5fcde327c879683293af8255511af827cbd
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787548"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="7ecf7-103">раздел: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="7ecf7-103">section: copyToNotebook</span></span>

<span data-ttu-id="7ecf7-104">Пространство имен: microsoft.graph копирует раздел в определенный блокнот.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-104">Namespace: microsoft.graph Copies a section to a specific notebook.</span></span>

<span data-ttu-id="7ecf7-105">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ecf7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ecf7-106">Permissions</span></span>
<span data-ttu-id="7ecf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ecf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ecf7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ecf7-109">Permission type</span></span>      | <span data-ttu-id="7ecf7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ecf7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ecf7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ecf7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ecf7-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecf7-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ecf7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ecf7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ecf7-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ecf7-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7ecf7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ecf7-115">Application</span></span> | <span data-ttu-id="7ecf7-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecf7-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ecf7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ecf7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="7ecf7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ecf7-118">Request headers</span></span>
| <span data-ttu-id="7ecf7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7ecf7-119">Name</span></span>       | <span data-ttu-id="7ecf7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7ecf7-120">Type</span></span> | <span data-ttu-id="7ecf7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ecf7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ecf7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ecf7-122">Authorization</span></span>  | <span data-ttu-id="7ecf7-123">string</span><span class="sxs-lookup"><span data-stu-id="7ecf7-123">string</span></span>  | <span data-ttu-id="7ecf7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ecf7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ecf7-126">Content-Type</span></span> | <span data-ttu-id="7ecf7-127">string</span><span class="sxs-lookup"><span data-stu-id="7ecf7-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7ecf7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ecf7-128">Request body</span></span>
<span data-ttu-id="7ecf7-129">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="7ecf7-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ecf7-130">Parameter</span></span>    | <span data-ttu-id="7ecf7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ecf7-131">Type</span></span>   |<span data-ttu-id="7ecf7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ecf7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ecf7-133">groupId</span><span class="sxs-lookup"><span data-stu-id="7ecf7-133">groupId</span></span>|<span data-ttu-id="7ecf7-134">String</span><span class="sxs-lookup"><span data-stu-id="7ecf7-134">String</span></span>|<span data-ttu-id="7ecf7-135">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-135">The id of the group to copy to.</span></span> <span data-ttu-id="7ecf7-136">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="7ecf7-137">id</span><span class="sxs-lookup"><span data-stu-id="7ecf7-137">id</span></span>|<span data-ttu-id="7ecf7-138">String</span><span class="sxs-lookup"><span data-stu-id="7ecf7-138">String</span></span>|<span data-ttu-id="7ecf7-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-139">Required.</span></span> <span data-ttu-id="7ecf7-140">ID записной книжки назначения.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-140">The id of the destination notebook.</span></span> |
|<span data-ttu-id="7ecf7-141">переименоватьAs</span><span class="sxs-lookup"><span data-stu-id="7ecf7-141">renameAs</span></span>|<span data-ttu-id="7ecf7-142">String</span><span class="sxs-lookup"><span data-stu-id="7ecf7-142">String</span></span>|<span data-ttu-id="7ecf7-143">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-143">The name of the copy.</span></span> <span data-ttu-id="7ecf7-144">По умолчанию имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-144">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="7ecf7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ecf7-145">Response</span></span>

<span data-ttu-id="7ecf7-146">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="7ecf7-147">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="7ecf7-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="7ecf7-148">Пример</span><span class="sxs-lookup"><span data-stu-id="7ecf7-148">Example</span></span>
<span data-ttu-id="7ecf7-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ecf7-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ecf7-150">Request</span></span>
<span data-ttu-id="7ecf7-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ecf7-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ecf7-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7ecf7-153">C#</span><span class="sxs-lookup"><span data-stu-id="7ecf7-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytonotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ecf7-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ecf7-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytonotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ecf7-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ecf7-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytonotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ecf7-156">Java</span><span class="sxs-lookup"><span data-stu-id="7ecf7-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytonotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ecf7-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ecf7-157">Response</span></span>
<span data-ttu-id="7ecf7-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ecf7-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

