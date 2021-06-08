---
title: 'блокнот: copyNotebook'
description: Копирует записную книжку в папку Notebooks в библиотеке документов назначения. Папка создается, если ее нет.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6f22838e9af2103f83f2c065e1376f931152fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786135"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="9745a-104">блокнот: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="9745a-104">notebook: copyNotebook</span></span>

<span data-ttu-id="9745a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9745a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9745a-106">Копирует записную книжку в папку Notebooks в библиотеке документов назначения.</span><span class="sxs-lookup"><span data-stu-id="9745a-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="9745a-107">Папка создается, если ее нет.</span><span class="sxs-lookup"><span data-stu-id="9745a-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="9745a-108">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="9745a-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="9745a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9745a-109">Permissions</span></span>
<span data-ttu-id="9745a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9745a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9745a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9745a-112">Permission type</span></span>      | <span data-ttu-id="9745a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9745a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9745a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9745a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9745a-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9745a-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9745a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9745a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9745a-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9745a-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9745a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9745a-118">Application</span></span> | <span data-ttu-id="9745a-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9745a-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9745a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9745a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="9745a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9745a-121">Request headers</span></span>
| <span data-ttu-id="9745a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9745a-122">Name</span></span>       | <span data-ttu-id="9745a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9745a-123">Type</span></span> | <span data-ttu-id="9745a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9745a-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9745a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9745a-125">Authorization</span></span>  | <span data-ttu-id="9745a-126">string</span><span class="sxs-lookup"><span data-stu-id="9745a-126">string</span></span>  | <span data-ttu-id="9745a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9745a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9745a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9745a-129">Content-Type</span></span> | <span data-ttu-id="9745a-130">string</span><span class="sxs-lookup"><span data-stu-id="9745a-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9745a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9745a-131">Request body</span></span>
<span data-ttu-id="9745a-132">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="9745a-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="9745a-133">Если нет необходимости, можно отправить пустое тело.</span><span class="sxs-lookup"><span data-stu-id="9745a-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="9745a-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="9745a-134">Parameter</span></span>    | <span data-ttu-id="9745a-135">Тип</span><span class="sxs-lookup"><span data-stu-id="9745a-135">Type</span></span>   |<span data-ttu-id="9745a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9745a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9745a-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="9745a-137">siteCollectionId</span></span>|<span data-ttu-id="9745a-138">String</span><span class="sxs-lookup"><span data-stu-id="9745a-138">String</span></span>|<span data-ttu-id="9745a-139">ID сайта SharePoint скопировать.</span><span class="sxs-lookup"><span data-stu-id="9745a-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="9745a-140">Используйте только при копировании на SharePoint сайте.</span><span class="sxs-lookup"><span data-stu-id="9745a-140">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="9745a-141">siteId</span><span class="sxs-lookup"><span data-stu-id="9745a-141">siteId</span></span>|<span data-ttu-id="9745a-142">String</span><span class="sxs-lookup"><span data-stu-id="9745a-142">String</span></span>|<span data-ttu-id="9745a-143">ID веб-SharePoint для копирования.</span><span class="sxs-lookup"><span data-stu-id="9745a-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="9745a-144">Используйте только при копировании на SharePoint сайте.</span><span class="sxs-lookup"><span data-stu-id="9745a-144">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="9745a-145">groupId</span><span class="sxs-lookup"><span data-stu-id="9745a-145">groupId</span></span>|<span data-ttu-id="9745a-146">String</span><span class="sxs-lookup"><span data-stu-id="9745a-146">String</span></span>|<span data-ttu-id="9745a-147">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="9745a-147">The id of the group to copy to.</span></span> <span data-ttu-id="9745a-148">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="9745a-148">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="9745a-149">переименоватьAs</span><span class="sxs-lookup"><span data-stu-id="9745a-149">renameAs</span></span>|<span data-ttu-id="9745a-150">String</span><span class="sxs-lookup"><span data-stu-id="9745a-150">String</span></span>|<span data-ttu-id="9745a-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="9745a-151">The name of the copy.</span></span> <span data-ttu-id="9745a-152">По умолчанию имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="9745a-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="9745a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9745a-153">Response</span></span>

<span data-ttu-id="9745a-154">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="9745a-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="9745a-155">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="9745a-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="9745a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9745a-156">Example</span></span>
<span data-ttu-id="9745a-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9745a-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9745a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="9745a-158">Request</span></span>
<span data-ttu-id="9745a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9745a-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9745a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="9745a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[<span data-ttu-id="9745a-161">C#</span><span class="sxs-lookup"><span data-stu-id="9745a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9745a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9745a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9745a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9745a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9745a-164">Java</span><span class="sxs-lookup"><span data-stu-id="9745a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9745a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9745a-165">Response</span></span>
<span data-ttu-id="9745a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9745a-166">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


