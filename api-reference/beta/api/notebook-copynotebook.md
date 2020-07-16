---
title: 'Записная книжка: Включеныcopynotebook'
description: Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов. Если эта папка не существует, она будет создана.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 028b6b577e9a018be0cfc97264b6344b51dd8ed2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44894853"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="0e4de-104">Записная книжка: Включеныcopynotebook</span><span class="sxs-lookup"><span data-stu-id="0e4de-104">notebook: copyNotebook</span></span>

<span data-ttu-id="0e4de-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e4de-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e4de-106">Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов.</span><span class="sxs-lookup"><span data-stu-id="0e4de-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="0e4de-107">Если эта папка не существует, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="0e4de-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="0e4de-108">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="0e4de-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e4de-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e4de-109">Permissions</span></span>
<span data-ttu-id="0e4de-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e4de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e4de-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e4de-112">Permission type</span></span>      | <span data-ttu-id="0e4de-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e4de-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e4de-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e4de-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0e4de-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e4de-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e4de-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e4de-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e4de-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e4de-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0e4de-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e4de-118">Application</span></span> | <span data-ttu-id="0e4de-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e4de-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e4de-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e4de-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="0e4de-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e4de-121">Request headers</span></span>
| <span data-ttu-id="0e4de-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0e4de-122">Name</span></span>       | <span data-ttu-id="0e4de-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0e4de-123">Type</span></span> | <span data-ttu-id="0e4de-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0e4de-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e4de-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e4de-125">Authorization</span></span>  | <span data-ttu-id="0e4de-126">string</span><span class="sxs-lookup"><span data-stu-id="0e4de-126">string</span></span>  | <span data-ttu-id="0e4de-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e4de-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e4de-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e4de-129">Content-Type</span></span> | <span data-ttu-id="0e4de-130">строка</span><span class="sxs-lookup"><span data-stu-id="0e4de-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0e4de-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e4de-131">Request body</span></span>
<span data-ttu-id="0e4de-132">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="0e4de-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="0e4de-133">Вы можете отправить пустой текст, если он не нужен.</span><span class="sxs-lookup"><span data-stu-id="0e4de-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="0e4de-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="0e4de-134">Parameter</span></span>    | <span data-ttu-id="0e4de-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0e4de-135">Type</span></span>   |<span data-ttu-id="0e4de-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0e4de-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e4de-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="0e4de-137">siteCollectionId</span></span>|<span data-ttu-id="0e4de-138">String</span><span class="sxs-lookup"><span data-stu-id="0e4de-138">String</span></span>|<span data-ttu-id="0e4de-139">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="0e4de-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="0e4de-140">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0e4de-140">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="0e4de-141">siteId</span><span class="sxs-lookup"><span data-stu-id="0e4de-141">siteId</span></span>|<span data-ttu-id="0e4de-142">String</span><span class="sxs-lookup"><span data-stu-id="0e4de-142">String</span></span>|<span data-ttu-id="0e4de-143">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="0e4de-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="0e4de-144">Используйте только при копировании на сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0e4de-144">Use only when copying to a SharePoint site.</span></span>|
|<span data-ttu-id="0e4de-145">groupId</span><span class="sxs-lookup"><span data-stu-id="0e4de-145">groupId</span></span>|<span data-ttu-id="0e4de-146">String</span><span class="sxs-lookup"><span data-stu-id="0e4de-146">String</span></span>|<span data-ttu-id="0e4de-147">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="0e4de-147">The id of the group to copy to.</span></span> <span data-ttu-id="0e4de-148">Используйте только при копировании в группу Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0e4de-148">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="0e4de-149">ренамеас</span><span class="sxs-lookup"><span data-stu-id="0e4de-149">renameAs</span></span>|<span data-ttu-id="0e4de-150">String</span><span class="sxs-lookup"><span data-stu-id="0e4de-150">String</span></span>|<span data-ttu-id="0e4de-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="0e4de-151">The name of the copy.</span></span> <span data-ttu-id="0e4de-152">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="0e4de-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="0e4de-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e4de-153">Response</span></span>

<span data-ttu-id="0e4de-154">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и `Operation-Location` заголовок.</span><span class="sxs-lookup"><span data-stu-id="0e4de-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="0e4de-155">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="0e4de-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="0e4de-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0e4de-156">Example</span></span>
<span data-ttu-id="0e4de-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0e4de-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e4de-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e4de-158">Request</span></span>
<span data-ttu-id="0e4de-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e4de-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e4de-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e4de-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0e4de-161">C#</span><span class="sxs-lookup"><span data-stu-id="0e4de-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e4de-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e4de-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e4de-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e4de-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e4de-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e4de-164">Response</span></span>
<span data-ttu-id="0e4de-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e4de-165">Here is an example of the response.</span></span>
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
