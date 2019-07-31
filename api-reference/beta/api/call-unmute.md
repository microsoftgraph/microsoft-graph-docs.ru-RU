---
title: 'вызов: включение звука'
description: Позволяет приложению включать и отключать микрофон.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83a309dd1ef321bb3149f2d3d0f9b2a48f33ee7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944396"
---
# <a name="call-unmute"></a><span data-ttu-id="69272-103">вызов: включение звука</span><span class="sxs-lookup"><span data-stu-id="69272-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69272-104">Позволяет приложению включать и отключать микрофон.</span><span class="sxs-lookup"><span data-stu-id="69272-104">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="69272-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69272-105">Permissions</span></span>
<span data-ttu-id="69272-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69272-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69272-108">Permission type</span></span>                        | <span data-ttu-id="69272-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69272-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="69272-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69272-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="69272-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69272-111">Not supported.</span></span>                               |
| <span data-ttu-id="69272-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69272-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69272-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69272-113">Not supported.</span></span>                               |
| <span data-ttu-id="69272-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="69272-114">Application</span></span>                            | <span data-ttu-id="69272-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69272-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="69272-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69272-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="69272-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69272-117">Request headers</span></span>
| <span data-ttu-id="69272-118">Имя</span><span class="sxs-lookup"><span data-stu-id="69272-118">Name</span></span>          | <span data-ttu-id="69272-119">Описание</span><span class="sxs-lookup"><span data-stu-id="69272-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="69272-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69272-120">Authorization</span></span> | <span data-ttu-id="69272-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69272-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69272-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69272-123">Request body</span></span>
<span data-ttu-id="69272-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="69272-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69272-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="69272-125">Parameter</span></span>      | <span data-ttu-id="69272-126">Тип</span><span class="sxs-lookup"><span data-stu-id="69272-126">Type</span></span>    |<span data-ttu-id="69272-127">Описание</span><span class="sxs-lookup"><span data-stu-id="69272-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69272-128">Контекст</span><span class="sxs-lookup"><span data-stu-id="69272-128">clientContext</span></span>|<span data-ttu-id="69272-129">String</span><span class="sxs-lookup"><span data-stu-id="69272-129">String</span></span>|<span data-ttu-id="69272-130">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="69272-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="69272-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="69272-131">Response</span></span>
<span data-ttu-id="69272-132">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69272-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69272-133">Пример</span><span class="sxs-lookup"><span data-stu-id="69272-133">Example</span></span>
<span data-ttu-id="69272-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="69272-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="69272-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="69272-135">Request</span></span>
<span data-ttu-id="69272-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69272-136">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="69272-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="69272-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69272-138">C#</span><span class="sxs-lookup"><span data-stu-id="69272-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69272-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="69272-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69272-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="69272-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="69272-141">Java</span><span class="sxs-lookup"><span data-stu-id="69272-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="69272-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="69272-142">Response</span></span>

> <span data-ttu-id="69272-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69272-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
