---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 7a916903a995badede8dba872e11614664151373
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788047"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="57bd5-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="57bd5-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="57bd5-104">Пространство имен: microsoft.graph копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="57bd5-104">Namespace: microsoft.graph Copies a section to a specific section group.</span></span>

<span data-ttu-id="57bd5-105">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="57bd5-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="57bd5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57bd5-106">Permissions</span></span>
<span data-ttu-id="57bd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57bd5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57bd5-109">Permission type</span></span>      | <span data-ttu-id="57bd5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57bd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57bd5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57bd5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57bd5-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57bd5-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="57bd5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57bd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57bd5-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57bd5-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="57bd5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57bd5-115">Application</span></span> | <span data-ttu-id="57bd5-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57bd5-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57bd5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57bd5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="57bd5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57bd5-118">Request headers</span></span>
| <span data-ttu-id="57bd5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57bd5-119">Name</span></span>       | <span data-ttu-id="57bd5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="57bd5-120">Type</span></span> | <span data-ttu-id="57bd5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="57bd5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57bd5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57bd5-122">Authorization</span></span>  | <span data-ttu-id="57bd5-123">string</span><span class="sxs-lookup"><span data-stu-id="57bd5-123">string</span></span>  | <span data-ttu-id="57bd5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57bd5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57bd5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57bd5-126">Content-Type</span></span> | <span data-ttu-id="57bd5-127">string</span><span class="sxs-lookup"><span data-stu-id="57bd5-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="57bd5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57bd5-128">Request body</span></span>
<span data-ttu-id="57bd5-129">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="57bd5-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="57bd5-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="57bd5-130">Parameter</span></span>    | <span data-ttu-id="57bd5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57bd5-131">Type</span></span>   |<span data-ttu-id="57bd5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57bd5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57bd5-133">groupId</span><span class="sxs-lookup"><span data-stu-id="57bd5-133">groupId</span></span>|<span data-ttu-id="57bd5-134">String</span><span class="sxs-lookup"><span data-stu-id="57bd5-134">String</span></span>|<span data-ttu-id="57bd5-135">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="57bd5-135">The id of the group to copy to.</span></span> <span data-ttu-id="57bd5-136">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="57bd5-136">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="57bd5-137">id</span><span class="sxs-lookup"><span data-stu-id="57bd5-137">id</span></span>|<span data-ttu-id="57bd5-138">String</span><span class="sxs-lookup"><span data-stu-id="57bd5-138">String</span></span>|<span data-ttu-id="57bd5-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57bd5-139">Required.</span></span> <span data-ttu-id="57bd5-140">ID группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="57bd5-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="57bd5-141">переименоватьAs</span><span class="sxs-lookup"><span data-stu-id="57bd5-141">renameAs</span></span>|<span data-ttu-id="57bd5-142">String</span><span class="sxs-lookup"><span data-stu-id="57bd5-142">String</span></span>|<span data-ttu-id="57bd5-143">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="57bd5-143">The name of the copy.</span></span> <span data-ttu-id="57bd5-144">По умолчанию имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="57bd5-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="57bd5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="57bd5-145">Response</span></span>

<span data-ttu-id="57bd5-146">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="57bd5-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="57bd5-147">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="57bd5-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="57bd5-148">Пример</span><span class="sxs-lookup"><span data-stu-id="57bd5-148">Example</span></span>
<span data-ttu-id="57bd5-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="57bd5-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57bd5-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="57bd5-150">Request</span></span>
<span data-ttu-id="57bd5-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57bd5-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57bd5-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="57bd5-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="57bd5-153">C#</span><span class="sxs-lookup"><span data-stu-id="57bd5-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57bd5-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57bd5-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57bd5-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57bd5-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57bd5-156">Java</span><span class="sxs-lookup"><span data-stu-id="57bd5-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="57bd5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="57bd5-157">Response</span></span>
<span data-ttu-id="57bd5-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57bd5-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

