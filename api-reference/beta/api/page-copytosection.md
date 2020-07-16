---
title: 'Страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2f37685212c48f3afe75a9c7daf2776f08aa92f6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896436"
---
# <a name="page-copytosection"></a><span data-ttu-id="5623e-103">Страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="5623e-103">page: copyToSection</span></span>

<span data-ttu-id="5623e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5623e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5623e-105">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="5623e-105">Copies a page to a specific section.</span></span>

<span data-ttu-id="5623e-106">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="5623e-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="5623e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5623e-107">Permissions</span></span>
<span data-ttu-id="5623e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5623e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5623e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5623e-110">Permission type</span></span>      | <span data-ttu-id="5623e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5623e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5623e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5623e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5623e-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5623e-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5623e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5623e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5623e-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5623e-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5623e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5623e-116">Application</span></span> | <span data-ttu-id="5623e-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5623e-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5623e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5623e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="5623e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5623e-119">Request headers</span></span>
| <span data-ttu-id="5623e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5623e-120">Name</span></span>       | <span data-ttu-id="5623e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5623e-121">Type</span></span> | <span data-ttu-id="5623e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5623e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5623e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5623e-123">Authorization</span></span>  | <span data-ttu-id="5623e-124">string</span><span class="sxs-lookup"><span data-stu-id="5623e-124">string</span></span>  | <span data-ttu-id="5623e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5623e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5623e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5623e-127">Content-Type</span></span> | <span data-ttu-id="5623e-128">строка</span><span class="sxs-lookup"><span data-stu-id="5623e-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5623e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5623e-129">Request body</span></span>
<span data-ttu-id="5623e-130">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="5623e-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="5623e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="5623e-131">Parameter</span></span>    | <span data-ttu-id="5623e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="5623e-132">Type</span></span>   |<span data-ttu-id="5623e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5623e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5623e-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="5623e-134">siteCollectionId</span></span>|<span data-ttu-id="5623e-135">String</span><span class="sxs-lookup"><span data-stu-id="5623e-135">String</span></span>|<span data-ttu-id="5623e-136">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="5623e-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="5623e-137">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5623e-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="5623e-138">siteId</span><span class="sxs-lookup"><span data-stu-id="5623e-138">siteId</span></span>|<span data-ttu-id="5623e-139">String</span><span class="sxs-lookup"><span data-stu-id="5623e-139">String</span></span>|<span data-ttu-id="5623e-140">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="5623e-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="5623e-141">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5623e-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="5623e-142">groupId</span><span class="sxs-lookup"><span data-stu-id="5623e-142">groupId</span></span>|<span data-ttu-id="5623e-143">String</span><span class="sxs-lookup"><span data-stu-id="5623e-143">String</span></span>|<span data-ttu-id="5623e-144">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="5623e-144">The id of the group to copy to.</span></span> <span data-ttu-id="5623e-145">Используйте только при копировании в группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5623e-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="5623e-146">id</span><span class="sxs-lookup"><span data-stu-id="5623e-146">id</span></span>|<span data-ttu-id="5623e-147">String</span><span class="sxs-lookup"><span data-stu-id="5623e-147">String</span></span>|<span data-ttu-id="5623e-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5623e-148">Required.</span></span> <span data-ttu-id="5623e-149">Идентификатор раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="5623e-149">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="5623e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5623e-150">Response</span></span>

<span data-ttu-id="5623e-151">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и `Operation-Location` заголовок.</span><span class="sxs-lookup"><span data-stu-id="5623e-151">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="5623e-152">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="5623e-152">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5623e-153">Пример</span><span class="sxs-lookup"><span data-stu-id="5623e-153">Example</span></span>
<span data-ttu-id="5623e-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5623e-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5623e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="5623e-155">Request</span></span>
<span data-ttu-id="5623e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5623e-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5623e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5623e-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5623e-158">C#</span><span class="sxs-lookup"><span data-stu-id="5623e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5623e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5623e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5623e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5623e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5623e-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="5623e-161">Response</span></span>
<span data-ttu-id="5623e-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5623e-162">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
