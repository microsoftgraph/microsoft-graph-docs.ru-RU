---
title: 'Call: Упдатеметадата'
description: Обновление метаданных апплиатион, связанных с вызовом.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e681ebf65ebed550d4180788eb5d534723981463
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636689"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="8dba6-103">Call: Упдатеметадата</span><span class="sxs-lookup"><span data-stu-id="8dba6-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dba6-104">Обновление метаданных апплиатион, связанных с вызовом.</span><span class="sxs-lookup"><span data-stu-id="8dba6-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dba6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dba6-105">Permissions</span></span>
<span data-ttu-id="8dba6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dba6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dba6-108">Permission type</span></span>                        | <span data-ttu-id="8dba6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dba6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dba6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dba6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dba6-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8dba6-111">Not Supported</span></span>                               |
| <span data-ttu-id="8dba6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dba6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dba6-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8dba6-113">Not Supported</span></span>                               |
| <span data-ttu-id="8dba6-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dba6-114">Application</span></span>     | <span data-ttu-id="8dba6-115">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="8dba6-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dba6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dba6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /communications/calls/{id}/updateMetadata
```
> <span data-ttu-id="8dba6-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8dba6-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8dba6-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="8dba6-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dba6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dba6-119">Request headers</span></span>
| <span data-ttu-id="8dba6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8dba6-120">Name</span></span>          | <span data-ttu-id="8dba6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8dba6-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8dba6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dba6-122">Authorization</span></span> | <span data-ttu-id="8dba6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dba6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dba6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dba6-125">Request body</span></span>
<span data-ttu-id="8dba6-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8dba6-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8dba6-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="8dba6-127">Parameter</span></span>      | <span data-ttu-id="8dba6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8dba6-128">Type</span></span>    |<span data-ttu-id="8dba6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8dba6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dba6-130">метаданных</span><span class="sxs-lookup"><span data-stu-id="8dba6-130">metadata</span></span>|<span data-ttu-id="8dba6-131">String</span><span class="sxs-lookup"><span data-stu-id="8dba6-131">String</span></span>|<span data-ttu-id="8dba6-132">Большой двоичный объект данных, предоставляемый участником в списке.</span><span class="sxs-lookup"><span data-stu-id="8dba6-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="8dba6-133">Контекст</span><span class="sxs-lookup"><span data-stu-id="8dba6-133">clientContext</span></span>|<span data-ttu-id="8dba6-134">String</span><span class="sxs-lookup"><span data-stu-id="8dba6-134">String</span></span>|<span data-ttu-id="8dba6-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="8dba6-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8dba6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dba6-136">Response</span></span>
<span data-ttu-id="8dba6-137">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="8dba6-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="8dba6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8dba6-138">Example</span></span>
<span data-ttu-id="8dba6-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8dba6-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8dba6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dba6-140">Request</span></span>
<span data-ttu-id="8dba6-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dba6-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8dba6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dba6-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8dba6-143">C#</span><span class="sxs-lookup"><span data-stu-id="8dba6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8dba6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dba6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8dba6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dba6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8dba6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dba6-146">Response</span></span>

> <span data-ttu-id="8dba6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dba6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
