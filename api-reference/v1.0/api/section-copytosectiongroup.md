---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9deb5c9003471026905457a910c6d966463df66b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021587"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="21a6a-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="21a6a-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="21a6a-104">Копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="21a6a-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="21a6a-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="21a6a-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="21a6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21a6a-106">Permissions</span></span>
<span data-ttu-id="21a6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21a6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21a6a-109">Permission type</span></span>      | <span data-ttu-id="21a6a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21a6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21a6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21a6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="21a6a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21a6a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="21a6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21a6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21a6a-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21a6a-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="21a6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21a6a-115">Application</span></span> | <span data-ttu-id="21a6a-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21a6a-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21a6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21a6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="21a6a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21a6a-118">Request headers</span></span>
| <span data-ttu-id="21a6a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="21a6a-119">Name</span></span>       | <span data-ttu-id="21a6a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="21a6a-120">Type</span></span> | <span data-ttu-id="21a6a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="21a6a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21a6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21a6a-122">Authorization</span></span>  | <span data-ttu-id="21a6a-123">string</span><span class="sxs-lookup"><span data-stu-id="21a6a-123">string</span></span>  | <span data-ttu-id="21a6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21a6a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21a6a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21a6a-126">Content-Type</span></span> | <span data-ttu-id="21a6a-127">строка</span><span class="sxs-lookup"><span data-stu-id="21a6a-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="21a6a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21a6a-128">Request body</span></span>
<span data-ttu-id="21a6a-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="21a6a-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="21a6a-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="21a6a-130">Parameter</span></span>    | <span data-ttu-id="21a6a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21a6a-131">Type</span></span>   |<span data-ttu-id="21a6a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21a6a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21a6a-133">groupId</span><span class="sxs-lookup"><span data-stu-id="21a6a-133">groupId</span></span>|<span data-ttu-id="21a6a-134">String</span><span class="sxs-lookup"><span data-stu-id="21a6a-134">String</span></span>|<span data-ttu-id="21a6a-135">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="21a6a-135">The id of the group to copy to.</span></span> <span data-ttu-id="21a6a-136">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="21a6a-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="21a6a-137">id</span><span class="sxs-lookup"><span data-stu-id="21a6a-137">id</span></span>|<span data-ttu-id="21a6a-138">String</span><span class="sxs-lookup"><span data-stu-id="21a6a-138">String</span></span>|<span data-ttu-id="21a6a-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21a6a-139">Required.</span></span> <span data-ttu-id="21a6a-140">Идентификатор группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="21a6a-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="21a6a-141">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="21a6a-141">renameAs</span></span>|<span data-ttu-id="21a6a-142">String</span><span class="sxs-lookup"><span data-stu-id="21a6a-142">String</span></span>|<span data-ttu-id="21a6a-143">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="21a6a-143">The name of the copy.</span></span> <span data-ttu-id="21a6a-144">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="21a6a-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="21a6a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a6a-145">Response</span></span>

<span data-ttu-id="21a6a-146">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="21a6a-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="21a6a-147">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="21a6a-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="21a6a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="21a6a-148">Example</span></span>
<span data-ttu-id="21a6a-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="21a6a-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="21a6a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="21a6a-150">Request</span></span>
<span data-ttu-id="21a6a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21a6a-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21a6a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="21a6a-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="21a6a-153">C#</span><span class="sxs-lookup"><span data-stu-id="21a6a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21a6a-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="21a6a-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21a6a-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="21a6a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21a6a-156">Java</span><span class="sxs-lookup"><span data-stu-id="21a6a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="21a6a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a6a-157">Response</span></span>
<span data-ttu-id="21a6a-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21a6a-158">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
