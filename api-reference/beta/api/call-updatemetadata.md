---
title: 'вызов: updateMetadata'
description: Обновление приложений метаданные, связанные с помощью вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b3dade26dde72acd796cc3751df136fde4a4bbea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507987"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="e0a26-103">вызов: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="e0a26-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a26-104">Обновление приложений метаданные, связанные с помощью вызова.</span><span class="sxs-lookup"><span data-stu-id="e0a26-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0a26-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a26-105">Permissions</span></span>
<span data-ttu-id="e0a26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0a26-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a26-108">Permission type</span></span>                        | <span data-ttu-id="e0a26-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0a26-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0a26-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0a26-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0a26-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e0a26-111">Not Supported</span></span>                               |
| <span data-ttu-id="e0a26-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0a26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0a26-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e0a26-113">Not Supported</span></span>                               |
| <span data-ttu-id="e0a26-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0a26-114">Application</span></span>     | <span data-ttu-id="e0a26-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="e0a26-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0a26-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0a26-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="e0a26-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0a26-117">Request headers</span></span>
| <span data-ttu-id="e0a26-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e0a26-118">Name</span></span>          | <span data-ttu-id="e0a26-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e0a26-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e0a26-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0a26-120">Authorization</span></span> | <span data-ttu-id="e0a26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0a26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0a26-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0a26-123">Request body</span></span>
<span data-ttu-id="e0a26-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e0a26-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0a26-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="e0a26-125">Parameter</span></span>      | <span data-ttu-id="e0a26-126">Тип</span><span class="sxs-lookup"><span data-stu-id="e0a26-126">Type</span></span>    |<span data-ttu-id="e0a26-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e0a26-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a26-128">metadata</span><span class="sxs-lookup"><span data-stu-id="e0a26-128">metadata</span></span>|<span data-ttu-id="e0a26-129">String</span><span class="sxs-lookup"><span data-stu-id="e0a26-129">String</span></span>|<span data-ttu-id="e0a26-130">Большой двоичный объект данных, предоставленных участника в списке.</span><span class="sxs-lookup"><span data-stu-id="e0a26-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="e0a26-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="e0a26-131">clientContext</span></span>|<span data-ttu-id="e0a26-132">String</span><span class="sxs-lookup"><span data-stu-id="e0a26-132">String</span></span>|<span data-ttu-id="e0a26-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="e0a26-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e0a26-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0a26-134">Response</span></span>
<span data-ttu-id="e0a26-135">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="e0a26-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="e0a26-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e0a26-136">Example</span></span>
<span data-ttu-id="e0a26-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e0a26-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e0a26-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0a26-138">Request</span></span>
<span data-ttu-id="e0a26-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0a26-139">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="e0a26-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0a26-140">Response</span></span>

> <span data-ttu-id="e0a26-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0a26-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-updatemetadata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
