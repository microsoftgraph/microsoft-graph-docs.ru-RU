---
title: 'page: copyToSection'
description: Копирование страницы в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: b09c47ab7dbaec7b7dd63d134cdefae1260d9e8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934823"
---
# <a name="page-copytosection"></a><span data-ttu-id="5ddbc-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="5ddbc-103">page: copyToSection</span></span>
<span data-ttu-id="5ddbc-104">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="5ddbc-105">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ddbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ddbc-106">Permissions</span></span>
<span data-ttu-id="5ddbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ddbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ddbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ddbc-109">Permission type</span></span>      | <span data-ttu-id="5ddbc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ddbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ddbc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ddbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ddbc-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ddbc-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ddbc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ddbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ddbc-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ddbc-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5ddbc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ddbc-115">Application</span></span> | <span data-ttu-id="5ddbc-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ddbc-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ddbc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ddbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="5ddbc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ddbc-118">Request headers</span></span>
| <span data-ttu-id="5ddbc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5ddbc-119">Name</span></span>       | <span data-ttu-id="5ddbc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5ddbc-120">Type</span></span> | <span data-ttu-id="5ddbc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5ddbc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ddbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ddbc-122">Authorization</span></span>  | <span data-ttu-id="5ddbc-123">string</span><span class="sxs-lookup"><span data-stu-id="5ddbc-123">string</span></span>  | <span data-ttu-id="5ddbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ddbc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ddbc-126">Content-Type</span></span> | <span data-ttu-id="5ddbc-127">string</span><span class="sxs-lookup"><span data-stu-id="5ddbc-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5ddbc-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ddbc-128">Request body</span></span>
<span data-ttu-id="5ddbc-129">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="5ddbc-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="5ddbc-130">Parameter</span></span>    | <span data-ttu-id="5ddbc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ddbc-131">Type</span></span>   |<span data-ttu-id="5ddbc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ddbc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ddbc-133">groupId</span><span class="sxs-lookup"><span data-stu-id="5ddbc-133">groupId</span></span>|<span data-ttu-id="5ddbc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5ddbc-134">String</span></span>|<span data-ttu-id="5ddbc-p103">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="5ddbc-137">id</span><span class="sxs-lookup"><span data-stu-id="5ddbc-137">id</span></span>|<span data-ttu-id="5ddbc-138">String</span><span class="sxs-lookup"><span data-stu-id="5ddbc-138">String</span></span>|<span data-ttu-id="5ddbc-p104">Обязательный. Идентификатор целевого раздела.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="5ddbc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ddbc-141">Response</span></span>

<span data-ttu-id="5ddbc-p105">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5ddbc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5ddbc-144">Example</span></span>
<span data-ttu-id="5ddbc-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ddbc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ddbc-146">Request</span></span>
<span data-ttu-id="5ddbc-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="5ddbc-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ddbc-148">Response</span></span>
<span data-ttu-id="5ddbc-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-149">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
