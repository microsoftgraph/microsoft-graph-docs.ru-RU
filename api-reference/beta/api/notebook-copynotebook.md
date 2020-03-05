---
title: 'Записная книжка: Включеныcopynotebook'
description: Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов. Если эта папка не существует, она будет создана.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 1e41a4893661a7995f57b81ec953ae0c42518ee5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456763"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="66807-104">Записная книжка: Включеныcopynotebook</span><span class="sxs-lookup"><span data-stu-id="66807-104">notebook: copyNotebook</span></span>

<span data-ttu-id="66807-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66807-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66807-106">Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов.</span><span class="sxs-lookup"><span data-stu-id="66807-106">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="66807-107">Если эта папка не существует, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="66807-107">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="66807-108">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="66807-108">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="66807-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66807-109">Permissions</span></span>
<span data-ttu-id="66807-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66807-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66807-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66807-112">Permission type</span></span>      | <span data-ttu-id="66807-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66807-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66807-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66807-114">Delegated (work or school account)</span></span> | <span data-ttu-id="66807-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66807-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="66807-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66807-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66807-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66807-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="66807-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66807-118">Application</span></span> | <span data-ttu-id="66807-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66807-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66807-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66807-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="66807-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66807-121">Request headers</span></span>
| <span data-ttu-id="66807-122">Имя</span><span class="sxs-lookup"><span data-stu-id="66807-122">Name</span></span>       | <span data-ttu-id="66807-123">Тип</span><span class="sxs-lookup"><span data-stu-id="66807-123">Type</span></span> | <span data-ttu-id="66807-124">Описание</span><span class="sxs-lookup"><span data-stu-id="66807-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66807-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="66807-125">Authorization</span></span>  | <span data-ttu-id="66807-126">string</span><span class="sxs-lookup"><span data-stu-id="66807-126">string</span></span>  | <span data-ttu-id="66807-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66807-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66807-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66807-129">Content-Type</span></span> | <span data-ttu-id="66807-130">строка</span><span class="sxs-lookup"><span data-stu-id="66807-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="66807-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66807-131">Request body</span></span>
<span data-ttu-id="66807-132">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="66807-132">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="66807-133">Вы можете отправить пустой текст, если он не нужен.</span><span class="sxs-lookup"><span data-stu-id="66807-133">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="66807-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="66807-134">Parameter</span></span>    | <span data-ttu-id="66807-135">Тип</span><span class="sxs-lookup"><span data-stu-id="66807-135">Type</span></span>   |<span data-ttu-id="66807-136">Описание</span><span class="sxs-lookup"><span data-stu-id="66807-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66807-137">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="66807-137">siteCollectionId</span></span>|<span data-ttu-id="66807-138">String</span><span class="sxs-lookup"><span data-stu-id="66807-138">String</span></span>|<span data-ttu-id="66807-139">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="66807-139">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="66807-140">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="66807-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="66807-141">siteId</span><span class="sxs-lookup"><span data-stu-id="66807-141">siteId</span></span>|<span data-ttu-id="66807-142">String</span><span class="sxs-lookup"><span data-stu-id="66807-142">String</span></span>|<span data-ttu-id="66807-143">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="66807-143">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="66807-144">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="66807-144">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="66807-145">groupId</span><span class="sxs-lookup"><span data-stu-id="66807-145">groupId</span></span>|<span data-ttu-id="66807-146">String</span><span class="sxs-lookup"><span data-stu-id="66807-146">String</span></span>|<span data-ttu-id="66807-147">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="66807-147">The id of the group to copy to.</span></span> <span data-ttu-id="66807-148">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="66807-148">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="66807-149">ренамеас</span><span class="sxs-lookup"><span data-stu-id="66807-149">renameAs</span></span>|<span data-ttu-id="66807-150">String</span><span class="sxs-lookup"><span data-stu-id="66807-150">String</span></span>|<span data-ttu-id="66807-151">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="66807-151">The name of the copy.</span></span> <span data-ttu-id="66807-152">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="66807-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="66807-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="66807-153">Response</span></span>

<span data-ttu-id="66807-154">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="66807-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="66807-155">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="66807-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="66807-156">Пример</span><span class="sxs-lookup"><span data-stu-id="66807-156">Example</span></span>
<span data-ttu-id="66807-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="66807-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66807-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="66807-158">Request</span></span>
<span data-ttu-id="66807-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66807-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66807-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="66807-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66807-161">C#</span><span class="sxs-lookup"><span data-stu-id="66807-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66807-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66807-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66807-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66807-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66807-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="66807-164">Response</span></span>
<span data-ttu-id="66807-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66807-165">Here is an example of the response.</span></span>
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
