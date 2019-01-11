---
title: 'page: copyToSection'
description: Копирование страницы в определенный раздел.
localization_priority: Normal
ms.openlocfilehash: 971d5eb47c6130ab7379e8b7db67d355b55c8d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871500"
---
# <a name="page-copytosection"></a><span data-ttu-id="d9abc-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="d9abc-103">page: copyToSection</span></span>
<span data-ttu-id="d9abc-104">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="d9abc-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="d9abc-105">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="d9abc-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9abc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9abc-106">Permissions</span></span>
<span data-ttu-id="d9abc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9abc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9abc-109">Permission type</span></span>      | <span data-ttu-id="d9abc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9abc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9abc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9abc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9abc-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9abc-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9abc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9abc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9abc-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9abc-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d9abc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9abc-115">Application</span></span> | <span data-ttu-id="d9abc-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9abc-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9abc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9abc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="d9abc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9abc-118">Request headers</span></span>
| <span data-ttu-id="d9abc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d9abc-119">Name</span></span>       | <span data-ttu-id="d9abc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d9abc-120">Type</span></span> | <span data-ttu-id="d9abc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9abc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9abc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9abc-122">Authorization</span></span>  | <span data-ttu-id="d9abc-123">string</span><span class="sxs-lookup"><span data-stu-id="d9abc-123">string</span></span>  | <span data-ttu-id="d9abc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9abc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9abc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9abc-126">Content-Type</span></span> | <span data-ttu-id="d9abc-127">string</span><span class="sxs-lookup"><span data-stu-id="d9abc-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d9abc-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9abc-128">Request body</span></span>
<span data-ttu-id="d9abc-129">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="d9abc-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="d9abc-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9abc-130">Parameter</span></span>    | <span data-ttu-id="d9abc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9abc-131">Type</span></span>   |<span data-ttu-id="d9abc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9abc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9abc-133">groupId</span><span class="sxs-lookup"><span data-stu-id="d9abc-133">groupId</span></span>|<span data-ttu-id="d9abc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d9abc-134">String</span></span>|<span data-ttu-id="d9abc-p103">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="d9abc-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="d9abc-137">id</span><span class="sxs-lookup"><span data-stu-id="d9abc-137">id</span></span>|<span data-ttu-id="d9abc-138">String</span><span class="sxs-lookup"><span data-stu-id="d9abc-138">String</span></span>|<span data-ttu-id="d9abc-p104">Обязательный. Идентификатор целевого раздела.</span><span class="sxs-lookup"><span data-stu-id="d9abc-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="d9abc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9abc-141">Response</span></span>

<span data-ttu-id="d9abc-p105">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="d9abc-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="d9abc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d9abc-144">Example</span></span>
<span data-ttu-id="d9abc-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d9abc-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9abc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9abc-146">Request</span></span>
<span data-ttu-id="d9abc-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9abc-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d9abc-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9abc-148">Response</span></span>
<span data-ttu-id="d9abc-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d9abc-149">Here is an example of the response.</span></span>
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
