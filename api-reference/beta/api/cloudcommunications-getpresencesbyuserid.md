---
title: 'Клаудкоммуникатионс: Жетпресенцесбюсерид'
description: Получение сведений о присутствии для нескольких пользователей.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 9480e85ad072d368b1afc768a859716865b78f75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982509"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="1c35a-103">Клаудкоммуникатионс: Жетпресенцесбюсерид</span><span class="sxs-lookup"><span data-stu-id="1c35a-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="1c35a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c35a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c35a-105">Получение сведений о [присутствии](../resources/presence.md) для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="1c35a-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c35a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c35a-106">Permissions</span></span>
<span data-ttu-id="1c35a-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="1c35a-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="1c35a-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c35a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c35a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c35a-109">Permission type</span></span> | <span data-ttu-id="1c35a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c35a-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1c35a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c35a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c35a-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c35a-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="1c35a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c35a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c35a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c35a-114">Not Supported.</span></span>                         |
| <span data-ttu-id="1c35a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c35a-115">Application</span></span>                            | <span data-ttu-id="1c35a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c35a-116">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1c35a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c35a-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="1c35a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c35a-118">Request Headers</span></span>
| <span data-ttu-id="1c35a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1c35a-119">Name</span></span>          | <span data-ttu-id="1c35a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1c35a-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1c35a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c35a-121">Authorization</span></span> | <span data-ttu-id="1c35a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c35a-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1c35a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c35a-124">Content-type</span></span> | <span data-ttu-id="1c35a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c35a-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1c35a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c35a-127">Request body</span></span>

<span data-ttu-id="1c35a-128">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="1c35a-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="1c35a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="1c35a-129">Parameter</span></span>      | <span data-ttu-id="1c35a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1c35a-130">Type</span></span>    |<span data-ttu-id="1c35a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1c35a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c35a-132">ids</span><span class="sxs-lookup"><span data-stu-id="1c35a-132">ids</span></span>|<span data-ttu-id="1c35a-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c35a-133">String collection</span></span>|<span data-ttu-id="1c35a-134">Идентификаторы объектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c35a-134">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="1c35a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c35a-135">Response</span></span>

<span data-ttu-id="1c35a-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c35a-136">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="1c35a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c35a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c35a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c35a-138">Request</span></span>
<span data-ttu-id="1c35a-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c35a-139">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c35a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c35a-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1c35a-141">C#</span><span class="sxs-lookup"><span data-stu-id="1c35a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c35a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c35a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c35a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c35a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1c35a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c35a-144">Response</span></span>
<span data-ttu-id="1c35a-145">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c35a-145">The following example shows the response.</span></span>

> <span data-ttu-id="1c35a-146">**Примечание:** Объекты ответа могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c35a-146">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="1c35a-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c35a-147">All the properties will be returned from an actual call.</span></span>

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


