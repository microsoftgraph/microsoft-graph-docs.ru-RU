---
title: 'Страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: fe8e0a18e91ecdad9daa648eb8a9944cad7a14de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992426"
---
# <a name="page-copytosection"></a><span data-ttu-id="ed705-103">Страница: copyToSection</span><span class="sxs-lookup"><span data-stu-id="ed705-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed705-104">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="ed705-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="ed705-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="ed705-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed705-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed705-106">Permissions</span></span>
<span data-ttu-id="ed705-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed705-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed705-109">Permission type</span></span>      | <span data-ttu-id="ed705-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed705-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed705-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed705-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed705-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed705-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed705-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed705-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed705-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed705-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ed705-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed705-115">Application</span></span> | <span data-ttu-id="ed705-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed705-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed705-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed705-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="ed705-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed705-118">Request headers</span></span>
| <span data-ttu-id="ed705-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ed705-119">Name</span></span>       | <span data-ttu-id="ed705-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ed705-120">Type</span></span> | <span data-ttu-id="ed705-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ed705-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed705-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed705-122">Authorization</span></span>  | <span data-ttu-id="ed705-123">string</span><span class="sxs-lookup"><span data-stu-id="ed705-123">string</span></span>  | <span data-ttu-id="ed705-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed705-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed705-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed705-126">Content-Type</span></span> | <span data-ttu-id="ed705-127">строка</span><span class="sxs-lookup"><span data-stu-id="ed705-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ed705-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed705-128">Request body</span></span>
<span data-ttu-id="ed705-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="ed705-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ed705-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ed705-130">Parameter</span></span>    | <span data-ttu-id="ed705-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ed705-131">Type</span></span>   |<span data-ttu-id="ed705-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ed705-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed705-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="ed705-133">siteCollectionId</span></span>|<span data-ttu-id="ed705-134">String</span><span class="sxs-lookup"><span data-stu-id="ed705-134">String</span></span>|<span data-ttu-id="ed705-135">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="ed705-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="ed705-136">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="ed705-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ed705-137">siteId</span><span class="sxs-lookup"><span data-stu-id="ed705-137">siteId</span></span>|<span data-ttu-id="ed705-138">String</span><span class="sxs-lookup"><span data-stu-id="ed705-138">String</span></span>|<span data-ttu-id="ed705-139">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="ed705-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="ed705-140">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="ed705-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ed705-141">groupId</span><span class="sxs-lookup"><span data-stu-id="ed705-141">groupId</span></span>|<span data-ttu-id="ed705-142">String</span><span class="sxs-lookup"><span data-stu-id="ed705-142">String</span></span>|<span data-ttu-id="ed705-143">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="ed705-143">The id of the group to copy to.</span></span> <span data-ttu-id="ed705-144">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="ed705-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="ed705-145">id</span><span class="sxs-lookup"><span data-stu-id="ed705-145">id</span></span>|<span data-ttu-id="ed705-146">String</span><span class="sxs-lookup"><span data-stu-id="ed705-146">String</span></span>|<span data-ttu-id="ed705-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed705-147">Required.</span></span> <span data-ttu-id="ed705-148">Идентификатор раздела назначения.</span><span class="sxs-lookup"><span data-stu-id="ed705-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="ed705-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed705-149">Response</span></span>

<span data-ttu-id="ed705-150">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="ed705-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="ed705-151">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="ed705-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ed705-152">Пример</span><span class="sxs-lookup"><span data-stu-id="ed705-152">Example</span></span>
<span data-ttu-id="ed705-153">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ed705-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed705-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed705-154">Request</span></span>
<span data-ttu-id="ed705-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed705-155">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed705-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed705-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed705-157">C#</span><span class="sxs-lookup"><span data-stu-id="ed705-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/page-copytosection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed705-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed705-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/page-copytosection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed705-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ed705-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/page-copytosection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ed705-160">Java</span><span class="sxs-lookup"><span data-stu-id="ed705-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/page-copytosection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed705-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed705-161">Response</span></span>
<span data-ttu-id="ed705-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed705-162">Here is an example of the response.</span></span>
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
