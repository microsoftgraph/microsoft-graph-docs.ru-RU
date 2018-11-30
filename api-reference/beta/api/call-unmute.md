---
title: 'Вызовите: Включение звука'
description: Позволяет приложениям включить сам.
ms.openlocfilehash: de2029a2fa5abeb777f83e8651c8b6c5a2c15991
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078219"
---
# <a name="call-unmute"></a><span data-ttu-id="889bf-103">Вызовите: Включение звука</span><span class="sxs-lookup"><span data-stu-id="889bf-103">call: unmute</span></span>

> <span data-ttu-id="889bf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="889bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="889bf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889bf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="889bf-106">Позволяет приложениям включить сам.</span><span class="sxs-lookup"><span data-stu-id="889bf-106">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="889bf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="889bf-107">Permissions</span></span>
<span data-ttu-id="889bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="889bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="889bf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="889bf-110">Permission type</span></span>                        | <span data-ttu-id="889bf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="889bf-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="889bf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="889bf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="889bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889bf-113">Not supported.</span></span>                               |
| <span data-ttu-id="889bf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="889bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="889bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889bf-115">Not supported.</span></span>                               |
| <span data-ttu-id="889bf-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="889bf-116">Application</span></span>                            | <span data-ttu-id="889bf-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="889bf-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="889bf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="889bf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="889bf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="889bf-119">Request headers</span></span>
| <span data-ttu-id="889bf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="889bf-120">Name</span></span>          | <span data-ttu-id="889bf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="889bf-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="889bf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="889bf-122">Authorization</span></span> | <span data-ttu-id="889bf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="889bf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="889bf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="889bf-125">Request body</span></span>
<span data-ttu-id="889bf-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="889bf-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="889bf-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="889bf-127">Parameter</span></span>      | <span data-ttu-id="889bf-128">Тип</span><span class="sxs-lookup"><span data-stu-id="889bf-128">Type</span></span>    |<span data-ttu-id="889bf-129">Description</span><span class="sxs-lookup"><span data-stu-id="889bf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="889bf-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="889bf-130">clientContext</span></span>|<span data-ttu-id="889bf-131">String</span><span class="sxs-lookup"><span data-stu-id="889bf-131">String</span></span>|<span data-ttu-id="889bf-132">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="889bf-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="889bf-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="889bf-133">Response</span></span>
<span data-ttu-id="889bf-134">Успешно завершена, этот метод возвращает `200 OK` объект [commsOperation](../resources/commsoperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="889bf-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="889bf-135">Пример</span><span class="sxs-lookup"><span data-stu-id="889bf-135">Example</span></span>
<span data-ttu-id="889bf-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="889bf-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="889bf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="889bf-137">Request</span></span>
<span data-ttu-id="889bf-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="889bf-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_unmute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="889bf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="889bf-139">Response</span></span>

> <span data-ttu-id="889bf-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="889bf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
