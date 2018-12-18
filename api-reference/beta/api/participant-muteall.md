---
title: 'Участник: muteAll'
description: Отключение всех участников в вызове.
author: VinodRavichandran
ms.openlocfilehash: 26369f3dc0c6502950c46ed1f9befe80ea1a320a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310180"
---
# <a name="participant-muteall"></a><span data-ttu-id="d9ba4-103">Участник: muteAll</span><span class="sxs-lookup"><span data-stu-id="d9ba4-103">participant: muteAll</span></span>

> <span data-ttu-id="d9ba4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9ba4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9ba4-106">Отключение всех участников в вызове.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-106">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9ba4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ba4-107">Permissions</span></span>
<span data-ttu-id="d9ba4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ba4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9ba4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ba4-110">Permission type</span></span>                        | <span data-ttu-id="d9ba4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9ba4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9ba4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9ba4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9ba4-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d9ba4-113">Not Supported</span></span>                               |
| <span data-ttu-id="d9ba4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9ba4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9ba4-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d9ba4-115">Not Supported</span></span>                               |
| <span data-ttu-id="d9ba4-116">Application</span><span class="sxs-lookup"><span data-stu-id="d9ba4-116">Application</span></span>                            | <span data-ttu-id="d9ba4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d9ba4-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="d9ba4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9ba4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="d9ba4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9ba4-119">Request headers</span></span>
| <span data-ttu-id="d9ba4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d9ba4-120">Name</span></span>          | <span data-ttu-id="d9ba4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ba4-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d9ba4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9ba4-122">Authorization</span></span> | <span data-ttu-id="d9ba4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9ba4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9ba4-125">Request body</span></span>
<span data-ttu-id="d9ba4-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9ba4-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9ba4-127">Parameter</span></span>      | <span data-ttu-id="d9ba4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ba4-128">Type</span></span>    |<span data-ttu-id="d9ba4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ba4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9ba4-130">participants</span><span class="sxs-lookup"><span data-stu-id="d9ba4-130">participants</span></span>|<span data-ttu-id="d9ba4-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9ba4-131">String collection</span></span>|<span data-ttu-id="d9ba4-132">Участники, выключен.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-132">The participants to be muted.</span></span>|
|<span data-ttu-id="d9ba4-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="d9ba4-133">clientContext</span></span>|<span data-ttu-id="d9ba4-134">String.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-134">String</span></span>|<span data-ttu-id="d9ba4-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="d9ba4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9ba4-136">Response</span></span>
<span data-ttu-id="d9ba4-137">Успешно завершена, этот метод возвращает `200 OK` объект [commsOperation](../resources/commsoperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-137">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ba4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d9ba4-138">Example</span></span>
<span data-ttu-id="d9ba4-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d9ba4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9ba4-140">Request</span></span>
<span data-ttu-id="d9ba4-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-141">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant_muteAll"
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

##### <a name="response"></a><span data-ttu-id="d9ba4-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9ba4-142">Response</span></span>

> <span data-ttu-id="d9ba4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9ba4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
