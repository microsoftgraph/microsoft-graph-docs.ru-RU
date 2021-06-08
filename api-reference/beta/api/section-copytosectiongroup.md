---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a75fcf7c2b52ff8309eb898f6f204186e06771de
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786751"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="beba0-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="beba0-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="beba0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beba0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beba0-105">Копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="beba0-105">Copies a section to a specific section group.</span></span>

<span data-ttu-id="beba0-106">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="beba0-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="beba0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beba0-107">Permissions</span></span>
<span data-ttu-id="beba0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beba0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beba0-110">Permission type</span></span>      | <span data-ttu-id="beba0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beba0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beba0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beba0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="beba0-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beba0-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="beba0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beba0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beba0-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="beba0-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="beba0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beba0-116">Application</span></span> | <span data-ttu-id="beba0-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beba0-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="beba0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beba0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="beba0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beba0-119">Request headers</span></span>
| <span data-ttu-id="beba0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="beba0-120">Name</span></span>       | <span data-ttu-id="beba0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="beba0-121">Type</span></span> | <span data-ttu-id="beba0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="beba0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="beba0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="beba0-123">Authorization</span></span>  | <span data-ttu-id="beba0-124">string</span><span class="sxs-lookup"><span data-stu-id="beba0-124">string</span></span>  | <span data-ttu-id="beba0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beba0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="beba0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="beba0-127">Content-Type</span></span> | <span data-ttu-id="beba0-128">string</span><span class="sxs-lookup"><span data-stu-id="beba0-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="beba0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beba0-129">Request body</span></span>
<span data-ttu-id="beba0-130">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="beba0-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="beba0-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="beba0-131">Parameter</span></span>    | <span data-ttu-id="beba0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="beba0-132">Type</span></span>   |<span data-ttu-id="beba0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="beba0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="beba0-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="beba0-134">siteCollectionId</span></span>|<span data-ttu-id="beba0-135">String</span><span class="sxs-lookup"><span data-stu-id="beba0-135">String</span></span>|<span data-ttu-id="beba0-136">ID сайта SharePoint скопировать.</span><span class="sxs-lookup"><span data-stu-id="beba0-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="beba0-137">Используйте только при копировании на SharePoint сайте.</span><span class="sxs-lookup"><span data-stu-id="beba0-137">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="beba0-138">siteId</span><span class="sxs-lookup"><span data-stu-id="beba0-138">siteId</span></span>|<span data-ttu-id="beba0-139">String</span><span class="sxs-lookup"><span data-stu-id="beba0-139">String</span></span>|<span data-ttu-id="beba0-140">ID веб-SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="beba0-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="beba0-141">Используйте только при копировании на SharePoint сайте.</span><span class="sxs-lookup"><span data-stu-id="beba0-141">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="beba0-142">groupId</span><span class="sxs-lookup"><span data-stu-id="beba0-142">groupId</span></span>|<span data-ttu-id="beba0-143">String</span><span class="sxs-lookup"><span data-stu-id="beba0-143">String</span></span>|<span data-ttu-id="beba0-144">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="beba0-144">The id of the group to copy to.</span></span> <span data-ttu-id="beba0-145">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="beba0-145">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="beba0-146">id</span><span class="sxs-lookup"><span data-stu-id="beba0-146">id</span></span>|<span data-ttu-id="beba0-147">String</span><span class="sxs-lookup"><span data-stu-id="beba0-147">String</span></span>|<span data-ttu-id="beba0-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beba0-148">Required.</span></span> <span data-ttu-id="beba0-149">ID группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="beba0-149">The id of the destination section group.</span></span> |
|<span data-ttu-id="beba0-150">переименоватьAs</span><span class="sxs-lookup"><span data-stu-id="beba0-150">renameAs</span></span>|<span data-ttu-id="beba0-151">String</span><span class="sxs-lookup"><span data-stu-id="beba0-151">String</span></span>|<span data-ttu-id="beba0-152">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="beba0-152">The name of the copy.</span></span> <span data-ttu-id="beba0-153">По умолчанию имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="beba0-153">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="beba0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="beba0-154">Response</span></span>

<span data-ttu-id="beba0-155">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="beba0-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="beba0-156">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="beba0-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="beba0-157">Пример</span><span class="sxs-lookup"><span data-stu-id="beba0-157">Example</span></span>
<span data-ttu-id="beba0-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="beba0-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="beba0-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="beba0-159">Request</span></span>
<span data-ttu-id="beba0-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beba0-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="beba0-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="beba0-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="beba0-162">C#</span><span class="sxs-lookup"><span data-stu-id="beba0-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="beba0-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beba0-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="beba0-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="beba0-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="beba0-165">Java</span><span class="sxs-lookup"><span data-stu-id="beba0-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/section-copytosectiongroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="beba0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="beba0-166">Response</span></span>
<span data-ttu-id="beba0-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="beba0-167">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


