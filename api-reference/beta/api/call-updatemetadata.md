---
title: 'Call: Упдатеметадата'
description: Обновление метаданных апплиатион, связанных с вызовом.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a336fe5f8327c6deba57c2f7aad2cb951cfa0e19
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635745"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="b7266-103">Call: Упдатеметадата</span><span class="sxs-lookup"><span data-stu-id="b7266-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7266-104">Обновление метаданных апплиатион, связанных с вызовом.</span><span class="sxs-lookup"><span data-stu-id="b7266-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7266-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7266-105">Permissions</span></span>
<span data-ttu-id="b7266-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7266-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7266-108">Permission type</span></span>                        | <span data-ttu-id="b7266-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7266-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b7266-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7266-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7266-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b7266-111">Not Supported</span></span>                               |
| <span data-ttu-id="b7266-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7266-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7266-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b7266-113">Not Supported</span></span>                               |
| <span data-ttu-id="b7266-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7266-114">Application</span></span>     | <span data-ttu-id="b7266-115">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="b7266-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7266-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7266-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="b7266-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7266-117">Request headers</span></span>
| <span data-ttu-id="b7266-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b7266-118">Name</span></span>          | <span data-ttu-id="b7266-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b7266-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b7266-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7266-120">Authorization</span></span> | <span data-ttu-id="b7266-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7266-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7266-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7266-123">Request body</span></span>
<span data-ttu-id="b7266-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b7266-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7266-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b7266-125">Parameter</span></span>      | <span data-ttu-id="b7266-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b7266-126">Type</span></span>    |<span data-ttu-id="b7266-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b7266-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7266-128">метаданных</span><span class="sxs-lookup"><span data-stu-id="b7266-128">metadata</span></span>|<span data-ttu-id="b7266-129">String</span><span class="sxs-lookup"><span data-stu-id="b7266-129">String</span></span>|<span data-ttu-id="b7266-130">Большой двоичный объект данных, предоставляемый участником в списке.</span><span class="sxs-lookup"><span data-stu-id="b7266-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="b7266-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="b7266-131">clientContext</span></span>|<span data-ttu-id="b7266-132">String</span><span class="sxs-lookup"><span data-stu-id="b7266-132">String</span></span>|<span data-ttu-id="b7266-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b7266-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b7266-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7266-134">Response</span></span>
<span data-ttu-id="b7266-135">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="b7266-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b7266-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b7266-136">Example</span></span>
<span data-ttu-id="b7266-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b7266-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b7266-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7266-138">Request</span></span>
<span data-ttu-id="b7266-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7266-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="b7266-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7266-140">Response</span></span>

> <span data-ttu-id="b7266-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7266-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b7266-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b7266-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b7266-144">Языках</span><span class="sxs-lookup"><span data-stu-id="b7266-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-updateMetadata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7266-145">Язык</span><span class="sxs-lookup"><span data-stu-id="b7266-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-updateMetadata-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/call-updatemetadata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-updatemetadata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
