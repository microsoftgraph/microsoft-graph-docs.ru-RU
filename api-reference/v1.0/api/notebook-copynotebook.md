---
title: 'notebook: copyNotebook'
description: Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.
ms.openlocfilehash: d3289f4f22a683d82605d01cc0355dba7ca72f29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026135"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="bf767-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="bf767-104">notebook: copyNotebook</span></span>
<span data-ttu-id="bf767-p102">Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="bf767-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="bf767-107">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="bf767-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf767-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf767-108">Permissions</span></span>
<span data-ttu-id="bf767-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf767-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf767-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf767-111">Permission type</span></span>      | <span data-ttu-id="bf767-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf767-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf767-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf767-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bf767-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf767-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf767-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf767-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf767-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf767-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="bf767-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf767-117">Application</span></span> | <span data-ttu-id="bf767-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf767-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf767-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf767-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="bf767-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf767-120">Request headers</span></span>
| <span data-ttu-id="bf767-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bf767-121">Name</span></span>       | <span data-ttu-id="bf767-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bf767-122">Type</span></span> | <span data-ttu-id="bf767-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bf767-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf767-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf767-124">Authorization</span></span>  | <span data-ttu-id="bf767-125">string</span><span class="sxs-lookup"><span data-stu-id="bf767-125">string</span></span>  | <span data-ttu-id="bf767-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf767-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf767-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf767-128">Content-Type</span></span> | <span data-ttu-id="bf767-129">string</span><span class="sxs-lookup"><span data-stu-id="bf767-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="bf767-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf767-130">Request body</span></span>
<span data-ttu-id="bf767-p105">В теле запроса укажите объект JSON, который содержит параметры, требуемые операцией. Если тело не нужно, можно отправить пустое тело.</span><span class="sxs-lookup"><span data-stu-id="bf767-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="bf767-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="bf767-133">Parameter</span></span>    | <span data-ttu-id="bf767-134">Тип</span><span class="sxs-lookup"><span data-stu-id="bf767-134">Type</span></span>   |<span data-ttu-id="bf767-135">Описание</span><span class="sxs-lookup"><span data-stu-id="bf767-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf767-136">groupId</span><span class="sxs-lookup"><span data-stu-id="bf767-136">groupId</span></span>|<span data-ttu-id="bf767-137">String</span><span class="sxs-lookup"><span data-stu-id="bf767-137">String</span></span>|<span data-ttu-id="bf767-p106">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="bf767-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="bf767-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="bf767-140">renameAs</span></span>|<span data-ttu-id="bf767-141">String</span><span class="sxs-lookup"><span data-stu-id="bf767-141">String</span></span>|<span data-ttu-id="bf767-p107">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="bf767-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="bf767-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf767-144">Response</span></span>

<span data-ttu-id="bf767-p108">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="bf767-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="bf767-147">Пример</span><span class="sxs-lookup"><span data-stu-id="bf767-147">Example</span></span>
<span data-ttu-id="bf767-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bf767-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf767-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf767-149">Request</span></span>
<span data-ttu-id="bf767-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf767-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="bf767-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf767-151">Response</span></span>
<span data-ttu-id="bf767-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf767-152">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
