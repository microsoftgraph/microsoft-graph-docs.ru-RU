---
title: 'section: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e122f8f7dfee82caa026ff569899516af4205ac2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991057"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="38cc6-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="38cc6-103">section: copyToNotebook</span></span>
<span data-ttu-id="38cc6-104">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="38cc6-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="38cc6-105">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="38cc6-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="38cc6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38cc6-106">Permissions</span></span>
<span data-ttu-id="38cc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38cc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38cc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38cc6-109">Permission type</span></span>      | <span data-ttu-id="38cc6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38cc6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38cc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38cc6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38cc6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38cc6-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="38cc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38cc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38cc6-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38cc6-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="38cc6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38cc6-115">Application</span></span> | <span data-ttu-id="38cc6-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38cc6-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38cc6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38cc6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="38cc6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38cc6-118">Request headers</span></span>
| <span data-ttu-id="38cc6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="38cc6-119">Name</span></span>       | <span data-ttu-id="38cc6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="38cc6-120">Type</span></span> | <span data-ttu-id="38cc6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="38cc6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38cc6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38cc6-122">Authorization</span></span>  | <span data-ttu-id="38cc6-123">string</span><span class="sxs-lookup"><span data-stu-id="38cc6-123">string</span></span>  | <span data-ttu-id="38cc6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38cc6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38cc6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38cc6-126">Content-Type</span></span> | <span data-ttu-id="38cc6-127">string</span><span class="sxs-lookup"><span data-stu-id="38cc6-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="38cc6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38cc6-128">Request body</span></span>
<span data-ttu-id="38cc6-129">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="38cc6-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="38cc6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="38cc6-130">Parameter</span></span>    | <span data-ttu-id="38cc6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38cc6-131">Type</span></span>   |<span data-ttu-id="38cc6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38cc6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38cc6-133">groupId</span><span class="sxs-lookup"><span data-stu-id="38cc6-133">groupId</span></span>|<span data-ttu-id="38cc6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="38cc6-134">String</span></span>|<span data-ttu-id="38cc6-p103">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="38cc6-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="38cc6-137">id</span><span class="sxs-lookup"><span data-stu-id="38cc6-137">id</span></span>|<span data-ttu-id="38cc6-138">Строка</span><span class="sxs-lookup"><span data-stu-id="38cc6-138">String</span></span>|<span data-ttu-id="38cc6-p104">Обязательный. Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="38cc6-p104">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="38cc6-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="38cc6-141">renameAs</span></span>|<span data-ttu-id="38cc6-142">Строка</span><span class="sxs-lookup"><span data-stu-id="38cc6-142">String</span></span>|<span data-ttu-id="38cc6-p105">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="38cc6-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="38cc6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="38cc6-145">Response</span></span>

<span data-ttu-id="38cc6-p106">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="38cc6-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="38cc6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="38cc6-148">Example</span></span>
<span data-ttu-id="38cc6-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="38cc6-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38cc6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="38cc6-150">Request</span></span>
<span data-ttu-id="38cc6-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38cc6-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="38cc6-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="38cc6-152">Response</span></span>
<span data-ttu-id="38cc6-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38cc6-153">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
