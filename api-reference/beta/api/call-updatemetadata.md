---
title: 'вызов: updateMetadata'
description: Обновление приложений метаданные, связанные с помощью вызова.
ms.openlocfilehash: fbd43db654294c92d05a8c4c6f12d2118298ff5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076625"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="b9259-103">вызов: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="b9259-103">call: updateMetadata</span></span>

> <span data-ttu-id="b9259-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9259-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9259-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9259-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9259-106">Обновление приложений метаданные, связанные с помощью вызова.</span><span class="sxs-lookup"><span data-stu-id="b9259-106">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9259-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9259-107">Permissions</span></span>
<span data-ttu-id="b9259-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9259-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9259-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9259-110">Permission type</span></span>                        | <span data-ttu-id="b9259-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9259-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9259-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9259-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9259-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b9259-113">Not Supported</span></span>                               |
| <span data-ttu-id="b9259-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9259-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9259-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b9259-115">Not Supported</span></span>                               |
| <span data-ttu-id="b9259-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b9259-116">Application</span></span>     | <span data-ttu-id="b9259-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b9259-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9259-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9259-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="b9259-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9259-119">Request headers</span></span>
| <span data-ttu-id="b9259-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b9259-120">Name</span></span>          | <span data-ttu-id="b9259-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b9259-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9259-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9259-122">Authorization</span></span> | <span data-ttu-id="b9259-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9259-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9259-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9259-125">Request body</span></span>
<span data-ttu-id="b9259-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b9259-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9259-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9259-127">Parameter</span></span>      | <span data-ttu-id="b9259-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b9259-128">Type</span></span>    |<span data-ttu-id="b9259-129">Description</span><span class="sxs-lookup"><span data-stu-id="b9259-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9259-130">metadata</span><span class="sxs-lookup"><span data-stu-id="b9259-130">metadata</span></span>|<span data-ttu-id="b9259-131">String</span><span class="sxs-lookup"><span data-stu-id="b9259-131">String</span></span>|<span data-ttu-id="b9259-132">Большой двоичный объект данных, предоставленных участника в списке.</span><span class="sxs-lookup"><span data-stu-id="b9259-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="b9259-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="b9259-133">clientContext</span></span>|<span data-ttu-id="b9259-134">String</span><span class="sxs-lookup"><span data-stu-id="b9259-134">String</span></span>|<span data-ttu-id="b9259-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b9259-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b9259-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9259-136">Response</span></span>
<span data-ttu-id="b9259-137">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="b9259-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b9259-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b9259-138">Example</span></span>
<span data-ttu-id="b9259-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b9259-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b9259-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9259-140">Request</span></span>
<span data-ttu-id="b9259-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9259-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_updateMetadata"
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

##### <a name="response"></a><span data-ttu-id="b9259-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9259-142">Response</span></span>

> <span data-ttu-id="b9259-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9259-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
