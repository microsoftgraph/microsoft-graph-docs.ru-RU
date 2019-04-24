---
title: 'вызов: включение звука'
description: Позволяет приложению включать и отключать микрофон.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4fce2bb622a7780fde9b95b64969b234a53e3be3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462411"
---
# <a name="call-unmute"></a><span data-ttu-id="b9c57-103">вызов: включение звука</span><span class="sxs-lookup"><span data-stu-id="b9c57-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c57-104">Позволяет приложению включать и отключать микрофон.</span><span class="sxs-lookup"><span data-stu-id="b9c57-104">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9c57-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c57-105">Permissions</span></span>
<span data-ttu-id="b9c57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9c57-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c57-108">Permission type</span></span>                        | <span data-ttu-id="b9c57-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9c57-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9c57-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9c57-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9c57-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c57-111">Not supported.</span></span>                               |
| <span data-ttu-id="b9c57-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9c57-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c57-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c57-113">Not supported.</span></span>                               |
| <span data-ttu-id="b9c57-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9c57-114">Application</span></span>                            | <span data-ttu-id="b9c57-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9c57-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b9c57-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9c57-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="b9c57-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9c57-117">Request headers</span></span>
| <span data-ttu-id="b9c57-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b9c57-118">Name</span></span>          | <span data-ttu-id="b9c57-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c57-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9c57-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9c57-120">Authorization</span></span> | <span data-ttu-id="b9c57-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9c57-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9c57-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9c57-123">Request body</span></span>
<span data-ttu-id="b9c57-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b9c57-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9c57-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9c57-125">Parameter</span></span>      | <span data-ttu-id="b9c57-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b9c57-126">Type</span></span>    |<span data-ttu-id="b9c57-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c57-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9c57-128">Контекст</span><span class="sxs-lookup"><span data-stu-id="b9c57-128">clientContext</span></span>|<span data-ttu-id="b9c57-129">String</span><span class="sxs-lookup"><span data-stu-id="b9c57-129">String</span></span>|<span data-ttu-id="b9c57-130">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b9c57-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b9c57-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c57-131">Response</span></span>
<span data-ttu-id="b9c57-132">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9c57-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c57-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b9c57-133">Example</span></span>
<span data-ttu-id="b9c57-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b9c57-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b9c57-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9c57-135">Request</span></span>
<span data-ttu-id="b9c57-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9c57-136">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b9c57-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9c57-137">Response</span></span>

> <span data-ttu-id="b9c57-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9c57-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/call-unmute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
