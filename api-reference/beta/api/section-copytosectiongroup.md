---
title: 'раздел: copyToSectionGroup'
description: Копирует раздел в определенную группу разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6f905cf3dfa0b8fffc9be3ffff9f9a60086cfcbb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453690"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="4ad2e-103">раздел: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="4ad2e-103">section: copyToSectionGroup</span></span>

<span data-ttu-id="4ad2e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ad2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ad2e-105">Копирует раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-105">Copies a section to a specific section group.</span></span>

<span data-ttu-id="4ad2e-106">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-106">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ad2e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ad2e-107">Permissions</span></span>
<span data-ttu-id="4ad2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ad2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ad2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ad2e-110">Permission type</span></span>      | <span data-ttu-id="4ad2e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ad2e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ad2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ad2e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ad2e-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ad2e-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ad2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ad2e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ad2e-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ad2e-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4ad2e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ad2e-116">Application</span></span> | <span data-ttu-id="4ad2e-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ad2e-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ad2e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ad2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
POST /sites/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="4ad2e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ad2e-119">Request headers</span></span>
| <span data-ttu-id="4ad2e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4ad2e-120">Name</span></span>       | <span data-ttu-id="4ad2e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4ad2e-121">Type</span></span> | <span data-ttu-id="4ad2e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4ad2e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ad2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ad2e-123">Authorization</span></span>  | <span data-ttu-id="4ad2e-124">string</span><span class="sxs-lookup"><span data-stu-id="4ad2e-124">string</span></span>  | <span data-ttu-id="4ad2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ad2e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ad2e-127">Content-Type</span></span> | <span data-ttu-id="4ad2e-128">строка</span><span class="sxs-lookup"><span data-stu-id="4ad2e-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4ad2e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ad2e-129">Request body</span></span>
<span data-ttu-id="4ad2e-130">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-130">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="4ad2e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="4ad2e-131">Parameter</span></span>    | <span data-ttu-id="4ad2e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4ad2e-132">Type</span></span>   |<span data-ttu-id="4ad2e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4ad2e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ad2e-134">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="4ad2e-134">siteCollectionId</span></span>|<span data-ttu-id="4ad2e-135">String</span><span class="sxs-lookup"><span data-stu-id="4ad2e-135">String</span></span>|<span data-ttu-id="4ad2e-136">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-136">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="4ad2e-137">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-137">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="4ad2e-138">siteId</span><span class="sxs-lookup"><span data-stu-id="4ad2e-138">siteId</span></span>|<span data-ttu-id="4ad2e-139">String</span><span class="sxs-lookup"><span data-stu-id="4ad2e-139">String</span></span>|<span data-ttu-id="4ad2e-140">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-140">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="4ad2e-141">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-141">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="4ad2e-142">groupId</span><span class="sxs-lookup"><span data-stu-id="4ad2e-142">groupId</span></span>|<span data-ttu-id="4ad2e-143">String</span><span class="sxs-lookup"><span data-stu-id="4ad2e-143">String</span></span>|<span data-ttu-id="4ad2e-144">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-144">The id of the group to copy to.</span></span> <span data-ttu-id="4ad2e-145">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-145">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4ad2e-146">id</span><span class="sxs-lookup"><span data-stu-id="4ad2e-146">id</span></span>|<span data-ttu-id="4ad2e-147">String</span><span class="sxs-lookup"><span data-stu-id="4ad2e-147">String</span></span>|<span data-ttu-id="4ad2e-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-148">Required.</span></span> <span data-ttu-id="4ad2e-149">Идентификатор группы разделов назначения.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-149">The id of the destination section group.</span></span> |
|<span data-ttu-id="4ad2e-150">ренамеас</span><span class="sxs-lookup"><span data-stu-id="4ad2e-150">renameAs</span></span>|<span data-ttu-id="4ad2e-151">String</span><span class="sxs-lookup"><span data-stu-id="4ad2e-151">String</span></span>|<span data-ttu-id="4ad2e-152">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-152">The name of the copy.</span></span> <span data-ttu-id="4ad2e-153">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-153">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="4ad2e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad2e-154">Response</span></span>

<span data-ttu-id="4ad2e-155">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-155">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="4ad2e-156">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="4ad2e-156">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4ad2e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="4ad2e-157">Example</span></span>
<span data-ttu-id="4ad2e-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ad2e-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ad2e-159">Request</span></span>
<span data-ttu-id="4ad2e-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ad2e-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ad2e-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4ad2e-162">C#</span><span class="sxs-lookup"><span data-stu-id="4ad2e-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/section-copytosectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ad2e-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ad2e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/section-copytosectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ad2e-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ad2e-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/section-copytosectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ad2e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad2e-165">Response</span></span>
<span data-ttu-id="4ad2e-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ad2e-166">Here is an example of the response.</span></span>
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
