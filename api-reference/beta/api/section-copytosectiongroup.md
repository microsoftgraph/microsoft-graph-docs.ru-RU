---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a9a0106b27ec2efeca6ee0cb0b7ec9dfaed0d829
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982935"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="61e0a-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="61e0a-103">section: copyToSectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61e0a-104">Копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="61e0a-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="61e0a-105">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="61e0a-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="61e0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61e0a-106">Permissions</span></span>
<span data-ttu-id="61e0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61e0a-109">Permission type</span></span>      | <span data-ttu-id="61e0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61e0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61e0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61e0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61e0a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e0a-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="61e0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61e0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61e0a-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61e0a-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="61e0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61e0a-115">Application</span></span> | <span data-ttu-id="61e0a-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e0a-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61e0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61e0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="61e0a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61e0a-118">Request headers</span></span>
| <span data-ttu-id="61e0a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="61e0a-119">Name</span></span>       | <span data-ttu-id="61e0a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="61e0a-120">Type</span></span> | <span data-ttu-id="61e0a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="61e0a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="61e0a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61e0a-122">Authorization</span></span>  | <span data-ttu-id="61e0a-123">string</span><span class="sxs-lookup"><span data-stu-id="61e0a-123">string</span></span>  | <span data-ttu-id="61e0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61e0a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61e0a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61e0a-126">Content-Type</span></span> | <span data-ttu-id="61e0a-127">строка</span><span class="sxs-lookup"><span data-stu-id="61e0a-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="61e0a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61e0a-128">Request body</span></span>
<span data-ttu-id="61e0a-129">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="61e0a-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="61e0a-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="61e0a-130">Parameter</span></span>    | <span data-ttu-id="61e0a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="61e0a-131">Type</span></span>   |<span data-ttu-id="61e0a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="61e0a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61e0a-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="61e0a-133">siteCollectionId</span></span>|<span data-ttu-id="61e0a-134">String</span><span class="sxs-lookup"><span data-stu-id="61e0a-134">String</span></span>|<span data-ttu-id="61e0a-135">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="61e0a-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="61e0a-136">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="61e0a-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="61e0a-137">siteId</span><span class="sxs-lookup"><span data-stu-id="61e0a-137">siteId</span></span>|<span data-ttu-id="61e0a-138">String</span><span class="sxs-lookup"><span data-stu-id="61e0a-138">String</span></span>|<span data-ttu-id="61e0a-139">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="61e0a-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="61e0a-140">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="61e0a-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="61e0a-141">groupId</span><span class="sxs-lookup"><span data-stu-id="61e0a-141">groupId</span></span>|<span data-ttu-id="61e0a-142">String</span><span class="sxs-lookup"><span data-stu-id="61e0a-142">String</span></span>|<span data-ttu-id="61e0a-143">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="61e0a-143">The id of the group to copy to.</span></span> <span data-ttu-id="61e0a-144">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="61e0a-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="61e0a-145">id</span><span class="sxs-lookup"><span data-stu-id="61e0a-145">id</span></span>|<span data-ttu-id="61e0a-146">String</span><span class="sxs-lookup"><span data-stu-id="61e0a-146">String</span></span>|<span data-ttu-id="61e0a-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61e0a-147">Required.</span></span> <span data-ttu-id="61e0a-148">Идентификатор группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="61e0a-148">The id of the destination section group.</span></span> |
|<span data-ttu-id="61e0a-149">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="61e0a-149">renameAs</span></span>|<span data-ttu-id="61e0a-150">String</span><span class="sxs-lookup"><span data-stu-id="61e0a-150">String</span></span>|<span data-ttu-id="61e0a-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="61e0a-151">The name of the copy.</span></span> <span data-ttu-id="61e0a-152">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="61e0a-152">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="61e0a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e0a-153">Response</span></span>

<span data-ttu-id="61e0a-154">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="61e0a-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="61e0a-155">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="61e0a-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="61e0a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="61e0a-156">Example</span></span>
<span data-ttu-id="61e0a-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="61e0a-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="61e0a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="61e0a-158">Request</span></span>
<span data-ttu-id="61e0a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61e0a-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="61e0a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="61e0a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61e0a-161">C#</span><span class="sxs-lookup"><span data-stu-id="61e0a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61e0a-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="61e0a-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61e0a-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="61e0a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="61e0a-164">Java</span><span class="sxs-lookup"><span data-stu-id="61e0a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="61e0a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e0a-165">Response</span></span>
<span data-ttu-id="61e0a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="61e0a-166">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
