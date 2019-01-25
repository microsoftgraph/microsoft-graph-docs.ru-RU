---
title: 'Вызовите: Выкл.'
description: Позволяет отключить самого приложения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f619cdc42ff914999ad8826ff31452ff82ea6a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524081"
---
# <a name="call-mute"></a><span data-ttu-id="c01c3-103">Вызовите: Выкл.</span><span class="sxs-lookup"><span data-stu-id="c01c3-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c01c3-104">Позволяет отключить самого приложения.</span><span class="sxs-lookup"><span data-stu-id="c01c3-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="c01c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c01c3-105">Permissions</span></span>
<span data-ttu-id="c01c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c01c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c01c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c01c3-108">Permission type</span></span>                        | <span data-ttu-id="c01c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c01c3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c01c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c01c3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c01c3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c01c3-111">Not Supported.</span></span>                               |
| <span data-ttu-id="c01c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c01c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c01c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c01c3-113">Not Supported.</span></span>                               |
| <span data-ttu-id="c01c3-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="c01c3-114">Application</span></span>                            | <span data-ttu-id="c01c3-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c01c3-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="c01c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c01c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="c01c3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c01c3-117">Request headers</span></span>
| <span data-ttu-id="c01c3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c01c3-118">Name</span></span>          | <span data-ttu-id="c01c3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c01c3-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c01c3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c01c3-120">Authorization</span></span> | <span data-ttu-id="c01c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c01c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c01c3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c01c3-123">Request body</span></span>
<span data-ttu-id="c01c3-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c01c3-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c01c3-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c01c3-125">Parameter</span></span>      | <span data-ttu-id="c01c3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c01c3-126">Type</span></span>    |<span data-ttu-id="c01c3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c01c3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c01c3-128">ClientContext</span><span class="sxs-lookup"><span data-stu-id="c01c3-128">clientContext</span></span>|<span data-ttu-id="c01c3-129">String</span><span class="sxs-lookup"><span data-stu-id="c01c3-129">String</span></span>|<span data-ttu-id="c01c3-130">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="c01c3-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="c01c3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c01c3-131">Response</span></span>
<span data-ttu-id="c01c3-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [commsOperation](../resources/commsoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c01c3-132">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c01c3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c01c3-133">Example</span></span>
<span data-ttu-id="c01c3-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c01c3-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c01c3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c01c3-135">Request</span></span>
<span data-ttu-id="c01c3-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c01c3-136">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c01c3-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c01c3-137">Response</span></span>

> <span data-ttu-id="c01c3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c01c3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-mute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
