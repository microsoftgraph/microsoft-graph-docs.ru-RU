---
title: 'вызов: выкл.'
description: Позволяет приложению отключить себя.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 50792a4a7cabe83780a6ca313a495e4ff1a8e71f
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635857"
---
# <a name="call-mute"></a><span data-ttu-id="fb926-103">вызов: выкл.</span><span class="sxs-lookup"><span data-stu-id="fb926-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb926-104">Позволяет приложению отключить себя.</span><span class="sxs-lookup"><span data-stu-id="fb926-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb926-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb926-105">Permissions</span></span>
<span data-ttu-id="fb926-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb926-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb926-108">Permission type</span></span>                        | <span data-ttu-id="fb926-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb926-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fb926-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb926-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb926-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb926-111">Not Supported.</span></span>                               |
| <span data-ttu-id="fb926-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb926-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb926-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb926-113">Not Supported.</span></span>                               |
| <span data-ttu-id="fb926-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="fb926-114">Application</span></span>                            | <span data-ttu-id="fb926-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fb926-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="fb926-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb926-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="fb926-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb926-117">Request headers</span></span>
| <span data-ttu-id="fb926-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fb926-118">Name</span></span>          | <span data-ttu-id="fb926-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fb926-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fb926-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb926-120">Authorization</span></span> | <span data-ttu-id="fb926-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb926-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb926-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb926-123">Request body</span></span>
<span data-ttu-id="fb926-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fb926-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fb926-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="fb926-125">Parameter</span></span>      | <span data-ttu-id="fb926-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fb926-126">Type</span></span>    |<span data-ttu-id="fb926-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fb926-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb926-128">Контекст</span><span class="sxs-lookup"><span data-stu-id="fb926-128">clientContext</span></span>|<span data-ttu-id="fb926-129">String</span><span class="sxs-lookup"><span data-stu-id="fb926-129">String</span></span>|<span data-ttu-id="fb926-130">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="fb926-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="fb926-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb926-131">Response</span></span>
<span data-ttu-id="fb926-132">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb926-132">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb926-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fb926-133">Example</span></span>
<span data-ttu-id="fb926-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fb926-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fb926-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb926-135">Request</span></span>
<span data-ttu-id="fb926-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb926-136">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="fb926-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb926-137">Response</span></span>

> <span data-ttu-id="fb926-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb926-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fb926-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="fb926-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fb926-141">Языках</span><span class="sxs-lookup"><span data-stu-id="fb926-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-mute-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb926-142">Язык</span><span class="sxs-lookup"><span data-stu-id="fb926-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-mute-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-mute.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-mute.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
