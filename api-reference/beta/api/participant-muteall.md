---
title: 'Участник: muteAll'
description: Отключение всех участников в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2a74a224141b77f0a09718bbafee3cf1dab0e8e9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522835"
---
# <a name="participant-muteall"></a><span data-ttu-id="1c19b-103">Участник: muteAll</span><span class="sxs-lookup"><span data-stu-id="1c19b-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c19b-104">Отключение всех участников в вызове.</span><span class="sxs-lookup"><span data-stu-id="1c19b-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c19b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c19b-105">Permissions</span></span>
<span data-ttu-id="1c19b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c19b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c19b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c19b-108">Permission type</span></span>                        | <span data-ttu-id="1c19b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c19b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c19b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c19b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c19b-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c19b-111">Not Supported</span></span>                               |
| <span data-ttu-id="1c19b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c19b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c19b-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c19b-113">Not Supported</span></span>                               |
| <span data-ttu-id="1c19b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c19b-114">Application</span></span>                            | <span data-ttu-id="1c19b-115">Нет</span><span class="sxs-lookup"><span data-stu-id="1c19b-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="1c19b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c19b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="1c19b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c19b-117">Request headers</span></span>
| <span data-ttu-id="1c19b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1c19b-118">Name</span></span>          | <span data-ttu-id="1c19b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1c19b-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1c19b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c19b-120">Authorization</span></span> | <span data-ttu-id="1c19b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c19b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c19b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c19b-123">Request body</span></span>
<span data-ttu-id="1c19b-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1c19b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c19b-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="1c19b-125">Parameter</span></span>      | <span data-ttu-id="1c19b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1c19b-126">Type</span></span>    |<span data-ttu-id="1c19b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1c19b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c19b-128">participants</span><span class="sxs-lookup"><span data-stu-id="1c19b-128">participants</span></span>|<span data-ttu-id="1c19b-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c19b-129">String collection</span></span>|<span data-ttu-id="1c19b-130">Участники, выключен.</span><span class="sxs-lookup"><span data-stu-id="1c19b-130">The participants to be muted.</span></span>|
|<span data-ttu-id="1c19b-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="1c19b-131">clientContext</span></span>|<span data-ttu-id="1c19b-132">String</span><span class="sxs-lookup"><span data-stu-id="1c19b-132">String</span></span>|<span data-ttu-id="1c19b-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="1c19b-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="1c19b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c19b-134">Response</span></span>
<span data-ttu-id="1c19b-135">Успешно завершена, этот метод возвращает `200 OK` объект [commsOperation](../resources/commsoperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c19b-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c19b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1c19b-136">Example</span></span>
<span data-ttu-id="1c19b-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1c19b-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1c19b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c19b-138">Request</span></span>
<span data-ttu-id="1c19b-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c19b-139">The following example shows the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1c19b-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c19b-140">Response</span></span>

> <span data-ttu-id="1c19b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c19b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/participant-muteall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
