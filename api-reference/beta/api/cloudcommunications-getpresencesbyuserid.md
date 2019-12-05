---
title: 'Клаудкоммуникатионс: Жетпресенцесбюсерид'
description: Получение сведений о присутствии для нескольких пользователей.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 5303c39584822a68afa559eb99c9fa579121e515
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844150"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="8c359-103">Клаудкоммуникатионс: Жетпресенцесбюсерид</span><span class="sxs-lookup"><span data-stu-id="8c359-103">cloudCommunications: getPresencesByUserId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c359-104">Получение сведений о [присутствии](../resources/presence.md) для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="8c359-104">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c359-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c359-105">Permissions</span></span>
<span data-ttu-id="8c359-106">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="8c359-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="8c359-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c359-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c359-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c359-108">Permission type</span></span> | <span data-ttu-id="8c359-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c359-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="8c359-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c359-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c359-111">Присутствие. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8c359-111">Presence.Read.All</span></span>                         |
| <span data-ttu-id="8c359-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c359-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c359-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c359-113">Not Supported.</span></span>                         |
| <span data-ttu-id="8c359-114">Application</span><span class="sxs-lookup"><span data-stu-id="8c359-114">Application</span></span>                            | <span data-ttu-id="8c359-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c359-115">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8c359-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c359-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="8c359-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c359-117">Request Headers</span></span>
| <span data-ttu-id="8c359-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8c359-118">Name</span></span>          | <span data-ttu-id="8c359-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8c359-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8c359-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c359-120">Authorization</span></span> | <span data-ttu-id="8c359-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c359-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8c359-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c359-123">Content-type</span></span> | <span data-ttu-id="8c359-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c359-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8c359-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c359-126">Request body</span></span>

<span data-ttu-id="8c359-127">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="8c359-127">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="8c359-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="8c359-128">Parameter</span></span>      | <span data-ttu-id="8c359-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8c359-129">Type</span></span>    |<span data-ttu-id="8c359-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8c359-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c359-131">ids</span><span class="sxs-lookup"><span data-stu-id="8c359-131">ids</span></span>|<span data-ttu-id="8c359-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8c359-132">String collection</span></span>|<span data-ttu-id="8c359-133">Идентификаторы объектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c359-133">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="8c359-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c359-134">Response</span></span>

<span data-ttu-id="8c359-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c359-135">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="8c359-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c359-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c359-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c359-137">Request</span></span>
<span data-ttu-id="8c359-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c359-138">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
### <a name="response"></a><span data-ttu-id="8c359-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c359-139">Response</span></span>
<span data-ttu-id="8c359-140">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c359-140">The following example shows the response.</span></span>

> <span data-ttu-id="8c359-141">**Примечание:** Объекты ответа могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c359-141">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="8c359-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c359-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
