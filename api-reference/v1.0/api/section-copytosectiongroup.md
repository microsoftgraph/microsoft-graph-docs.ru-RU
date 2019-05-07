---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 56aaab6ad53318be6c943e526eb4cc8a9676c63f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603479"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="1bc0e-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="1bc0e-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="1bc0e-104">Копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="1bc0e-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bc0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc0e-106">Permissions</span></span>
<span data-ttu-id="1bc0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bc0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc0e-109">Permission type</span></span>      | <span data-ttu-id="1bc0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bc0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bc0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bc0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1bc0e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc0e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1bc0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bc0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc0e-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bc0e-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1bc0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bc0e-115">Application</span></span> | <span data-ttu-id="1bc0e-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc0e-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bc0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bc0e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="1bc0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bc0e-118">Request headers</span></span>
| <span data-ttu-id="1bc0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1bc0e-119">Name</span></span>       | <span data-ttu-id="1bc0e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1bc0e-120">Type</span></span> | <span data-ttu-id="1bc0e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc0e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bc0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc0e-122">Authorization</span></span>  | <span data-ttu-id="1bc0e-123">string</span><span class="sxs-lookup"><span data-stu-id="1bc0e-123">string</span></span>  | <span data-ttu-id="1bc0e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1bc0e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bc0e-126">Content-Type</span></span> | <span data-ttu-id="1bc0e-127">строка</span><span class="sxs-lookup"><span data-stu-id="1bc0e-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1bc0e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bc0e-128">Request body</span></span>
<span data-ttu-id="1bc0e-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="1bc0e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1bc0e-130">Parameter</span></span>    | <span data-ttu-id="1bc0e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1bc0e-131">Type</span></span>   |<span data-ttu-id="1bc0e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc0e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bc0e-133">groupId</span><span class="sxs-lookup"><span data-stu-id="1bc0e-133">groupId</span></span>|<span data-ttu-id="1bc0e-134">String</span><span class="sxs-lookup"><span data-stu-id="1bc0e-134">String</span></span>|<span data-ttu-id="1bc0e-135">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-135">The id of the group to copy to.</span></span> <span data-ttu-id="1bc0e-136">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="1bc0e-137">id</span><span class="sxs-lookup"><span data-stu-id="1bc0e-137">id</span></span>|<span data-ttu-id="1bc0e-138">String</span><span class="sxs-lookup"><span data-stu-id="1bc0e-138">String</span></span>|<span data-ttu-id="1bc0e-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-139">Required.</span></span> <span data-ttu-id="1bc0e-140">Идентификатор группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="1bc0e-141">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="1bc0e-141">renameAs</span></span>|<span data-ttu-id="1bc0e-142">String</span><span class="sxs-lookup"><span data-stu-id="1bc0e-142">String</span></span>|<span data-ttu-id="1bc0e-143">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-143">The name of the copy.</span></span> <span data-ttu-id="1bc0e-144">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="1bc0e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc0e-145">Response</span></span>

<span data-ttu-id="1bc0e-146">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="1bc0e-147">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="1bc0e-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="1bc0e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="1bc0e-148">Example</span></span>
<span data-ttu-id="1bc0e-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1bc0e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bc0e-150">Request</span></span>
<span data-ttu-id="1bc0e-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1bc0e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc0e-152">Response</span></span>
<span data-ttu-id="1bc0e-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bc0e-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1bc0e-154">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1bc0e-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1bc0e-155">Языках</span><span class="sxs-lookup"><span data-stu-id="1bc0e-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bc0e-156">Язык</span><span class="sxs-lookup"><span data-stu-id="1bc0e-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
