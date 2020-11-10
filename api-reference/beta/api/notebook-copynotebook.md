---
title: 'Записная книжка: Включеныcopynotebook'
description: Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов. Если эта папка не существует, она будет создана.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e591dcc436d336bc8b98db84385bd2974c83de7f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951556"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="7ff79-104">Записная книжка: Включеныcopynotebook</span><span class="sxs-lookup"><span data-stu-id="7ff79-104">notebook: copyNotebook</span></span>

<span data-ttu-id="7ff79-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff79-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff79-106">Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов.</span><span class="sxs-lookup"><span data-stu-id="7ff79-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="7ff79-107">Если эта папка не существует, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="7ff79-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="7ff79-108">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="7ff79-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ff79-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff79-109">Permissions</span></span>
<span data-ttu-id="7ff79-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff79-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff79-112">Permission type</span></span>      | <span data-ttu-id="7ff79-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ff79-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ff79-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ff79-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7ff79-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff79-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ff79-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ff79-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ff79-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ff79-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7ff79-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ff79-118">Application</span></span> | <span data-ttu-id="7ff79-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff79-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ff79-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ff79-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="7ff79-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ff79-121">Request headers</span></span>
| <span data-ttu-id="7ff79-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7ff79-122">Name</span></span>       | <span data-ttu-id="7ff79-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff79-123">Type</span></span> | <span data-ttu-id="7ff79-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff79-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ff79-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff79-125">Authorization</span></span>  | <span data-ttu-id="7ff79-126">string</span><span class="sxs-lookup"><span data-stu-id="7ff79-126">string</span></span>  | <span data-ttu-id="7ff79-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ff79-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ff79-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ff79-129">Content-Type</span></span> | <span data-ttu-id="7ff79-130">string</span><span class="sxs-lookup"><span data-stu-id="7ff79-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7ff79-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ff79-131">Request body</span></span>
<span data-ttu-id="7ff79-132">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="7ff79-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="7ff79-133">Вы можете отправить пустой текст, если он не нужен.</span><span class="sxs-lookup"><span data-stu-id="7ff79-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="7ff79-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ff79-134">Parameter</span></span>    | <span data-ttu-id="7ff79-135">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff79-135">Type</span></span>   |<span data-ttu-id="7ff79-136">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff79-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ff79-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="7ff79-137">siteCollectionId</span></span>|<span data-ttu-id="7ff79-138">String</span><span class="sxs-lookup"><span data-stu-id="7ff79-138">String</span></span>|<span data-ttu-id="7ff79-139">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="7ff79-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="7ff79-140">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7ff79-140">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="7ff79-141">siteId</span><span class="sxs-lookup"><span data-stu-id="7ff79-141">siteId</span></span>|<span data-ttu-id="7ff79-142">String</span><span class="sxs-lookup"><span data-stu-id="7ff79-142">String</span></span>|<span data-ttu-id="7ff79-143">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="7ff79-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="7ff79-144">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7ff79-144">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="7ff79-145">groupId</span><span class="sxs-lookup"><span data-stu-id="7ff79-145">groupId</span></span>|<span data-ttu-id="7ff79-146">String</span><span class="sxs-lookup"><span data-stu-id="7ff79-146">String</span></span>|<span data-ttu-id="7ff79-147">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="7ff79-147">The id of the group to copy to.</span></span> <span data-ttu-id="7ff79-148">Используйте только при копировании в группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7ff79-148">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="7ff79-149">ренамеас</span><span class="sxs-lookup"><span data-stu-id="7ff79-149">renameAs</span></span>|<span data-ttu-id="7ff79-150">String</span><span class="sxs-lookup"><span data-stu-id="7ff79-150">String</span></span>|<span data-ttu-id="7ff79-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="7ff79-151">The name of the copy.</span></span> <span data-ttu-id="7ff79-152">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="7ff79-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="7ff79-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff79-153">Response</span></span>

<span data-ttu-id="7ff79-154">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и `Operation-Location` заголовок.</span><span class="sxs-lookup"><span data-stu-id="7ff79-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="7ff79-155">Опрос конечной точки Operation-Location для [получения состояния операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="7ff79-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="7ff79-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7ff79-156">Example</span></span>
<span data-ttu-id="7ff79-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7ff79-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ff79-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff79-158">Request</span></span>
<span data-ttu-id="7ff79-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ff79-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff79-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff79-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7ff79-161">C#</span><span class="sxs-lookup"><span data-stu-id="7ff79-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff79-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff79-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff79-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff79-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ff79-164">Java</span><span class="sxs-lookup"><span data-stu-id="7ff79-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ff79-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff79-165">Response</span></span>
<span data-ttu-id="7ff79-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ff79-166">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


