---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 34455921995768ba9d2faffac3319cb1d58b5d64
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279305"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="4a2e9-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="4a2e9-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="4a2e9-104">Копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="4a2e9-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a2e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a2e9-106">Permissions</span></span>
<span data-ttu-id="4a2e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a2e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a2e9-109">Permission type</span></span>      | <span data-ttu-id="4a2e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a2e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a2e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a2e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a2e9-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2e9-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a2e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a2e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a2e9-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a2e9-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4a2e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a2e9-115">Application</span></span> | <span data-ttu-id="4a2e9-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2e9-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a2e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a2e9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="4a2e9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a2e9-118">Request headers</span></span>
| <span data-ttu-id="4a2e9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a2e9-119">Name</span></span>       | <span data-ttu-id="4a2e9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4a2e9-120">Type</span></span> | <span data-ttu-id="4a2e9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a2e9-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a2e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a2e9-122">Authorization</span></span>  | <span data-ttu-id="4a2e9-123">string</span><span class="sxs-lookup"><span data-stu-id="4a2e9-123">string</span></span>  | <span data-ttu-id="4a2e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a2e9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a2e9-126">Content-Type</span></span> | <span data-ttu-id="4a2e9-127">строка</span><span class="sxs-lookup"><span data-stu-id="4a2e9-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4a2e9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a2e9-128">Request body</span></span>
<span data-ttu-id="4a2e9-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="4a2e9-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a2e9-130">Parameter</span></span>    | <span data-ttu-id="4a2e9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a2e9-131">Type</span></span>   |<span data-ttu-id="4a2e9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a2e9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a2e9-133">groupId</span><span class="sxs-lookup"><span data-stu-id="4a2e9-133">groupId</span></span>|<span data-ttu-id="4a2e9-134">String</span><span class="sxs-lookup"><span data-stu-id="4a2e9-134">String</span></span>|<span data-ttu-id="4a2e9-135">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-135">The id of the group to copy to.</span></span> <span data-ttu-id="4a2e9-136">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4a2e9-137">id</span><span class="sxs-lookup"><span data-stu-id="4a2e9-137">id</span></span>|<span data-ttu-id="4a2e9-138">String</span><span class="sxs-lookup"><span data-stu-id="4a2e9-138">String</span></span>|<span data-ttu-id="4a2e9-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-139">Required.</span></span> <span data-ttu-id="4a2e9-140">Идентификатор группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="4a2e9-141">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="4a2e9-141">renameAs</span></span>|<span data-ttu-id="4a2e9-142">String</span><span class="sxs-lookup"><span data-stu-id="4a2e9-142">String</span></span>|<span data-ttu-id="4a2e9-143">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-143">The name of the copy.</span></span> <span data-ttu-id="4a2e9-144">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="4a2e9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a2e9-145">Response</span></span>

<span data-ttu-id="4a2e9-146">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="4a2e9-147">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="4a2e9-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4a2e9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4a2e9-148">Example</span></span>
<span data-ttu-id="4a2e9-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a2e9-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a2e9-150">Request</span></span>
<span data-ttu-id="4a2e9-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4a2e9-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a2e9-152">Response</span></span>
<span data-ttu-id="4a2e9-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a2e9-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a2e9-154">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4a2e9-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a2e9-155">C#</span><span class="sxs-lookup"><span data-stu-id="4a2e9-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a2e9-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a2e9-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4a2e9-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4a2e9-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
