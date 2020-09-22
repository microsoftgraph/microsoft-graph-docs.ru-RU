---
title: 'Call: Упдатеметадата'
description: Обновление метаданных апплиатион, связанных с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c31028880f9fc6160daf0d8a734f3efe28ad757f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987262"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="be148-103">Call: Упдатеметадата</span><span class="sxs-lookup"><span data-stu-id="be148-103">call: updateMetadata</span></span>

<span data-ttu-id="be148-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be148-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be148-105">Обновление метаданных апплиатион, связанных с вызовом.</span><span class="sxs-lookup"><span data-stu-id="be148-105">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="be148-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be148-106">Permissions</span></span>
<span data-ttu-id="be148-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be148-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be148-109">Permission type</span></span>                        | <span data-ttu-id="be148-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be148-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be148-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be148-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be148-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be148-112">Not Supported</span></span>                               |
| <span data-ttu-id="be148-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be148-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be148-114">Not Supported</span></span>                               |
| <span data-ttu-id="be148-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be148-115">Application</span></span>     | <span data-ttu-id="be148-116">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls.IniТиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="be148-116">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be148-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be148-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /communications/calls/{id}/updateMetadata
```
> <span data-ttu-id="be148-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="be148-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="be148-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="be148-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be148-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be148-120">Request headers</span></span>
| <span data-ttu-id="be148-121">Имя</span><span class="sxs-lookup"><span data-stu-id="be148-121">Name</span></span>          | <span data-ttu-id="be148-122">Описание</span><span class="sxs-lookup"><span data-stu-id="be148-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="be148-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be148-123">Authorization</span></span> | <span data-ttu-id="be148-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be148-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be148-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be148-126">Request body</span></span>
<span data-ttu-id="be148-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="be148-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be148-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="be148-128">Parameter</span></span>      | <span data-ttu-id="be148-129">Тип</span><span class="sxs-lookup"><span data-stu-id="be148-129">Type</span></span>    |<span data-ttu-id="be148-130">Описание</span><span class="sxs-lookup"><span data-stu-id="be148-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be148-131">метаданных</span><span class="sxs-lookup"><span data-stu-id="be148-131">metadata</span></span>|<span data-ttu-id="be148-132">String</span><span class="sxs-lookup"><span data-stu-id="be148-132">String</span></span>|<span data-ttu-id="be148-133">Большой двоичный объект данных, предоставляемый участником в списке.</span><span class="sxs-lookup"><span data-stu-id="be148-133">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="be148-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="be148-134">clientContext</span></span>|<span data-ttu-id="be148-135">String</span><span class="sxs-lookup"><span data-stu-id="be148-135">String</span></span>|<span data-ttu-id="be148-136">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="be148-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="be148-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="be148-137">Response</span></span>
<span data-ttu-id="be148-138">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="be148-138">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="be148-139">Пример</span><span class="sxs-lookup"><span data-stu-id="be148-139">Example</span></span>
<span data-ttu-id="be148-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="be148-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="be148-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="be148-141">Request</span></span>
<span data-ttu-id="be148-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be148-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be148-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="be148-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="be148-144">C#</span><span class="sxs-lookup"><span data-stu-id="be148-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be148-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be148-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be148-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be148-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be148-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="be148-147">Response</span></span>

> <span data-ttu-id="be148-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be148-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateMetadata",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


