---
title: 'Записная книжка: Включеныcopynotebook'
description: Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов. Если эта папка не существует, она будет создана.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: b0299f930d4059539d7e54eba45020f3fd7db2f9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597808"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="5573c-104">Записная книжка: Включеныcopynotebook</span><span class="sxs-lookup"><span data-stu-id="5573c-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5573c-105">Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов.</span><span class="sxs-lookup"><span data-stu-id="5573c-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="5573c-106">Если эта папка не существует, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="5573c-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="5573c-107">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="5573c-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="5573c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5573c-108">Permissions</span></span>
<span data-ttu-id="5573c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5573c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5573c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5573c-111">Permission type</span></span>      | <span data-ttu-id="5573c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5573c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5573c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5573c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5573c-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5573c-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5573c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5573c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5573c-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5573c-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5573c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5573c-117">Application</span></span> | <span data-ttu-id="5573c-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5573c-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5573c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5573c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="5573c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5573c-120">Request headers</span></span>
| <span data-ttu-id="5573c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5573c-121">Name</span></span>       | <span data-ttu-id="5573c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5573c-122">Type</span></span> | <span data-ttu-id="5573c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5573c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5573c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5573c-124">Authorization</span></span>  | <span data-ttu-id="5573c-125">string</span><span class="sxs-lookup"><span data-stu-id="5573c-125">string</span></span>  | <span data-ttu-id="5573c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5573c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5573c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5573c-128">Content-Type</span></span> | <span data-ttu-id="5573c-129">строка</span><span class="sxs-lookup"><span data-stu-id="5573c-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5573c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5573c-130">Request body</span></span>
<span data-ttu-id="5573c-131">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="5573c-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="5573c-132">Вы можете отправить пустой текст, если он не нужен.</span><span class="sxs-lookup"><span data-stu-id="5573c-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="5573c-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="5573c-133">Parameter</span></span>    | <span data-ttu-id="5573c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5573c-134">Type</span></span>   |<span data-ttu-id="5573c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5573c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5573c-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="5573c-136">siteCollectionId</span></span>|<span data-ttu-id="5573c-137">String</span><span class="sxs-lookup"><span data-stu-id="5573c-137">String</span></span>|<span data-ttu-id="5573c-138">Идентификатор сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="5573c-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="5573c-139">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="5573c-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="5573c-140">siteId</span><span class="sxs-lookup"><span data-stu-id="5573c-140">siteId</span></span>|<span data-ttu-id="5573c-141">String</span><span class="sxs-lookup"><span data-stu-id="5573c-141">String</span></span>|<span data-ttu-id="5573c-142">Идентификатор веб-сайта SharePoint, в который необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="5573c-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="5573c-143">Используйте только при копировании на сайт группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="5573c-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="5573c-144">groupId</span><span class="sxs-lookup"><span data-stu-id="5573c-144">groupId</span></span>|<span data-ttu-id="5573c-145">String</span><span class="sxs-lookup"><span data-stu-id="5573c-145">String</span></span>|<span data-ttu-id="5573c-146">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="5573c-146">The id of the group to copy to.</span></span> <span data-ttu-id="5573c-147">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="5573c-147">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="5573c-148">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="5573c-148">renameAs</span></span>|<span data-ttu-id="5573c-149">String</span><span class="sxs-lookup"><span data-stu-id="5573c-149">String</span></span>|<span data-ttu-id="5573c-150">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="5573c-150">The name of the copy.</span></span> <span data-ttu-id="5573c-151">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="5573c-151">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="5573c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5573c-152">Response</span></span>

<span data-ttu-id="5573c-153">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="5573c-153">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="5573c-154">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="5573c-154">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5573c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="5573c-155">Example</span></span>
<span data-ttu-id="5573c-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5573c-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5573c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5573c-157">Request</span></span>
<span data-ttu-id="5573c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5573c-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5573c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5573c-159">Response</span></span>
<span data-ttu-id="5573c-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5573c-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5573c-161">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5573c-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5573c-162">Языках</span><span class="sxs-lookup"><span data-stu-id="5573c-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5573c-163">Язык</span><span class="sxs-lookup"><span data-stu-id="5573c-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/notebook_copynotebook-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
