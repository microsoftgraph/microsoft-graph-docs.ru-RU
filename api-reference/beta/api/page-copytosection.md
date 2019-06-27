---
title: 'Страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 12b7a1fa807ac6c552e39506978f6aa929ac93d6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267776"
---
# <a name="page-copytosection"></a><span data-ttu-id="eb92e-103">Страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="eb92e-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb92e-104">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="eb92e-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="eb92e-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="eb92e-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb92e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb92e-106">Permissions</span></span>
<span data-ttu-id="eb92e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb92e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb92e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb92e-109">Permission type</span></span>      | <span data-ttu-id="eb92e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb92e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb92e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb92e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb92e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb92e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb92e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb92e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb92e-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb92e-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="eb92e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb92e-115">Application</span></span> | <span data-ttu-id="eb92e-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb92e-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb92e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb92e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="eb92e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb92e-118">Request headers</span></span>
| <span data-ttu-id="eb92e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eb92e-119">Name</span></span>       | <span data-ttu-id="eb92e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="eb92e-120">Type</span></span> | <span data-ttu-id="eb92e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eb92e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb92e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb92e-122">Authorization</span></span>  | <span data-ttu-id="eb92e-123">string</span><span class="sxs-lookup"><span data-stu-id="eb92e-123">string</span></span>  | <span data-ttu-id="eb92e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb92e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb92e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb92e-126">Content-Type</span></span> | <span data-ttu-id="eb92e-127">строка</span><span class="sxs-lookup"><span data-stu-id="eb92e-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="eb92e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb92e-128">Request body</span></span>
<span data-ttu-id="eb92e-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="eb92e-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="eb92e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="eb92e-130">Parameter</span></span>    | <span data-ttu-id="eb92e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eb92e-131">Type</span></span>   |<span data-ttu-id="eb92e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eb92e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb92e-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="eb92e-133">siteCollectionId</span></span>|<span data-ttu-id="eb92e-134">String</span><span class="sxs-lookup"><span data-stu-id="eb92e-134">String</span></span>|<span data-ttu-id="eb92e-135">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="eb92e-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="eb92e-136">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb92e-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="eb92e-137">siteId</span><span class="sxs-lookup"><span data-stu-id="eb92e-137">siteId</span></span>|<span data-ttu-id="eb92e-138">String</span><span class="sxs-lookup"><span data-stu-id="eb92e-138">String</span></span>|<span data-ttu-id="eb92e-139">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="eb92e-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="eb92e-140">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb92e-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="eb92e-141">groupId</span><span class="sxs-lookup"><span data-stu-id="eb92e-141">groupId</span></span>|<span data-ttu-id="eb92e-142">String</span><span class="sxs-lookup"><span data-stu-id="eb92e-142">String</span></span>|<span data-ttu-id="eb92e-143">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="eb92e-143">The id of the group to copy to.</span></span> <span data-ttu-id="eb92e-144">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb92e-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="eb92e-145">id</span><span class="sxs-lookup"><span data-stu-id="eb92e-145">id</span></span>|<span data-ttu-id="eb92e-146">String</span><span class="sxs-lookup"><span data-stu-id="eb92e-146">String</span></span>|<span data-ttu-id="eb92e-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb92e-147">Required.</span></span> <span data-ttu-id="eb92e-148">Идентификатор раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="eb92e-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="eb92e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb92e-149">Response</span></span>

<span data-ttu-id="eb92e-150">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="eb92e-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="eb92e-151">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="eb92e-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="eb92e-152">Пример</span><span class="sxs-lookup"><span data-stu-id="eb92e-152">Example</span></span>
<span data-ttu-id="eb92e-153">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="eb92e-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb92e-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb92e-154">Request</span></span>
<span data-ttu-id="eb92e-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb92e-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eb92e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb92e-156">Response</span></span>
<span data-ttu-id="eb92e-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb92e-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb92e-158">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="eb92e-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb92e-159">C#</span><span class="sxs-lookup"><span data-stu-id="eb92e-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/page_copytosection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb92e-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb92e-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/page_copytosection-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eb92e-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="eb92e-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/page_copytosection-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
