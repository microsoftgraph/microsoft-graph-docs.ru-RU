---
title: 'блокнот: copyNotebook'
description: Копирует записную книжку в папку Notebooks в библиотеке документов назначения. Папка создается, если ее нет.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f46e65f200e87d0f39ef5e9307ee199de5595fb1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787459"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="e982e-104">блокнот: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="e982e-104">notebook: copyNotebook</span></span>

<span data-ttu-id="e982e-105">Пространство имен: microsoft.graph копирует записную книжку в папку Блокноты в библиотеке документов назначения.</span><span class="sxs-lookup"><span data-stu-id="e982e-105">Namespace: microsoft.graph Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="e982e-106">Папка создается, если ее нет.</span><span class="sxs-lookup"><span data-stu-id="e982e-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="e982e-107">Для операций с копированием следует асинхронный шаблон вызова: сначала вызываем действие Copy, а затем опылите конечную точку операции для результата.</span><span class="sxs-lookup"><span data-stu-id="e982e-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="e982e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e982e-108">Permissions</span></span>
<span data-ttu-id="e982e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e982e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e982e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e982e-111">Permission type</span></span>      | <span data-ttu-id="e982e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e982e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e982e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e982e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e982e-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e982e-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e982e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e982e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e982e-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e982e-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e982e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e982e-117">Application</span></span> | <span data-ttu-id="e982e-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e982e-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e982e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e982e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="e982e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e982e-120">Request headers</span></span>
| <span data-ttu-id="e982e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e982e-121">Name</span></span>       | <span data-ttu-id="e982e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e982e-122">Type</span></span> | <span data-ttu-id="e982e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e982e-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e982e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e982e-124">Authorization</span></span>  | <span data-ttu-id="e982e-125">string</span><span class="sxs-lookup"><span data-stu-id="e982e-125">string</span></span>  | <span data-ttu-id="e982e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e982e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e982e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e982e-128">Content-Type</span></span> | <span data-ttu-id="e982e-129">string</span><span class="sxs-lookup"><span data-stu-id="e982e-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e982e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e982e-130">Request body</span></span>
<span data-ttu-id="e982e-131">В теле запроса укажи объект JSON, содержащий параметры, необходимые для операции.</span><span class="sxs-lookup"><span data-stu-id="e982e-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="e982e-132">Если нет необходимости, можно отправить пустое тело.</span><span class="sxs-lookup"><span data-stu-id="e982e-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="e982e-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="e982e-133">Parameter</span></span>    | <span data-ttu-id="e982e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e982e-134">Type</span></span>   |<span data-ttu-id="e982e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e982e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e982e-136">groupId</span><span class="sxs-lookup"><span data-stu-id="e982e-136">groupId</span></span>|<span data-ttu-id="e982e-137">String</span><span class="sxs-lookup"><span data-stu-id="e982e-137">String</span></span>|<span data-ttu-id="e982e-138">ID группы для копирования.</span><span class="sxs-lookup"><span data-stu-id="e982e-138">The id of the group to copy to.</span></span> <span data-ttu-id="e982e-139">Используйте только при копировании в Microsoft 365 группу.</span><span class="sxs-lookup"><span data-stu-id="e982e-139">Use only when copying to a Microsoft 365 group.</span></span>|
|<span data-ttu-id="e982e-140">переименоватьAs</span><span class="sxs-lookup"><span data-stu-id="e982e-140">renameAs</span></span>|<span data-ttu-id="e982e-141">String</span><span class="sxs-lookup"><span data-stu-id="e982e-141">String</span></span>|<span data-ttu-id="e982e-142">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="e982e-142">The name of the copy.</span></span> <span data-ttu-id="e982e-143">По умолчанию имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="e982e-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="e982e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e982e-144">Response</span></span>

<span data-ttu-id="e982e-145">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и `Operation-Location` загот.</span><span class="sxs-lookup"><span data-stu-id="e982e-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="e982e-146">Опрос конечной Operation-Location, [чтобы получить состояние операции копирования.](onenoteoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="e982e-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="e982e-147">Пример</span><span class="sxs-lookup"><span data-stu-id="e982e-147">Example</span></span>
<span data-ttu-id="e982e-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e982e-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e982e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e982e-149">Request</span></span>
<span data-ttu-id="e982e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e982e-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e982e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e982e-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e982e-152">C#</span><span class="sxs-lookup"><span data-stu-id="e982e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e982e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e982e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e982e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e982e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e982e-155">Java</span><span class="sxs-lookup"><span data-stu-id="e982e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e982e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e982e-156">Response</span></span>
<span data-ttu-id="e982e-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e982e-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

