---
title: 'участник: Мутеалл'
description: Отключение звука всех участников вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bdfe0b3f337b7f5a084e1f557d6fc66ae8b8f0f2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413743"
---
# <a name="participant-muteall"></a><span data-ttu-id="d0443-103">участник: Мутеалл</span><span class="sxs-lookup"><span data-stu-id="d0443-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0443-104">Отключение звука всех участников вызова.</span><span class="sxs-lookup"><span data-stu-id="d0443-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0443-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0443-105">Permissions</span></span>
<span data-ttu-id="d0443-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0443-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0443-108">Permission type</span></span>                        | <span data-ttu-id="d0443-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0443-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0443-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0443-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0443-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d0443-111">Not Supported</span></span>                               |
| <span data-ttu-id="d0443-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0443-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0443-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d0443-113">Not Supported</span></span>                               |
| <span data-ttu-id="d0443-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0443-114">Application</span></span>                            | <span data-ttu-id="d0443-115">Нет</span><span class="sxs-lookup"><span data-stu-id="d0443-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="d0443-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0443-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="d0443-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0443-117">Request headers</span></span>
| <span data-ttu-id="d0443-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d0443-118">Name</span></span>          | <span data-ttu-id="d0443-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d0443-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d0443-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0443-120">Authorization</span></span> | <span data-ttu-id="d0443-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0443-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0443-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0443-123">Request body</span></span>
<span data-ttu-id="d0443-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d0443-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d0443-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="d0443-125">Parameter</span></span>      | <span data-ttu-id="d0443-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d0443-126">Type</span></span>    |<span data-ttu-id="d0443-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d0443-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0443-128">participants</span><span class="sxs-lookup"><span data-stu-id="d0443-128">participants</span></span>|<span data-ttu-id="d0443-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d0443-129">String collection</span></span>|<span data-ttu-id="d0443-130">Участники, которые должны быть отключены.</span><span class="sxs-lookup"><span data-stu-id="d0443-130">The participants to be muted.</span></span>|
|<span data-ttu-id="d0443-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="d0443-131">clientContext</span></span>|<span data-ttu-id="d0443-132">String</span><span class="sxs-lookup"><span data-stu-id="d0443-132">String</span></span>|<span data-ttu-id="d0443-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="d0443-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="d0443-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0443-134">Response</span></span>
<span data-ttu-id="d0443-135">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0443-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0443-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d0443-136">Example</span></span>
<span data-ttu-id="d0443-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d0443-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d0443-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0443-138">Request</span></span>
<span data-ttu-id="d0443-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0443-139">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d0443-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0443-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d0443-141">C#</span><span class="sxs-lookup"><span data-stu-id="d0443-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0443-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0443-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0443-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d0443-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0443-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0443-144">Response</span></span>

> <span data-ttu-id="d0443-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0443-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
