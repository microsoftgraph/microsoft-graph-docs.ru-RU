---
title: 'cloudCommunications: getPresencesByUserId'
description: Получите сведения о присутствии для нескольких пользователей.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a3c6b0fe4d223ef458aad7d9b271cfdee37e590c
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796534"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="b01ba-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="b01ba-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="b01ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01ba-105">Получите сведения [о](../resources/presence.md) присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="b01ba-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="b01ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b01ba-106">Permissions</span></span>
<span data-ttu-id="b01ba-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b01ba-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="b01ba-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b01ba-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b01ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b01ba-109">Permission type</span></span> | <span data-ttu-id="b01ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b01ba-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b01ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b01ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b01ba-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01ba-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="b01ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b01ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b01ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b01ba-114">Not Supported.</span></span>                         |
| <span data-ttu-id="b01ba-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b01ba-115">Application</span></span>                            | <span data-ttu-id="b01ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b01ba-116">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="b01ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b01ba-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="b01ba-118">Заглавные запросы</span><span class="sxs-lookup"><span data-stu-id="b01ba-118">Request Headers</span></span>
| <span data-ttu-id="b01ba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b01ba-119">Name</span></span>          | <span data-ttu-id="b01ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b01ba-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b01ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b01ba-121">Authorization</span></span> | <span data-ttu-id="b01ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b01ba-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b01ba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b01ba-124">Content-type</span></span> | <span data-ttu-id="b01ba-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b01ba-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b01ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b01ba-127">Request body</span></span>

<span data-ttu-id="b01ba-128">В теле запроса укажу объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="b01ba-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="b01ba-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="b01ba-129">Parameter</span></span>      | <span data-ttu-id="b01ba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b01ba-130">Type</span></span>    |<span data-ttu-id="b01ba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b01ba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b01ba-132">ids</span><span class="sxs-lookup"><span data-stu-id="b01ba-132">ids</span></span>|<span data-ttu-id="b01ba-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b01ba-133">String collection</span></span>|<span data-ttu-id="b01ba-134">ИД объектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="b01ba-134">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="b01ba-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b01ba-135">Response</span></span>

<span data-ttu-id="b01ba-136">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b01ba-136">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="b01ba-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="b01ba-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b01ba-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b01ba-138">Request</span></span>
<span data-ttu-id="b01ba-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b01ba-139">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b01ba-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b01ba-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b01ba-141">C#</span><span class="sxs-lookup"><span data-stu-id="b01ba-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b01ba-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b01ba-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b01ba-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b01ba-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b01ba-144">Java</span><span class="sxs-lookup"><span data-stu-id="b01ba-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b01ba-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b01ba-145">Response</span></span>
<span data-ttu-id="b01ba-146">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b01ba-146">The following example shows the response.</span></span>

> <span data-ttu-id="b01ba-147">**Примечание.** Объекты ответа могут быть сокращены для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="b01ba-147">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="b01ba-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b01ba-148">All the properties will be returned from an actual call.</span></span>

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
      "activity": "InAMeeting",
      "outOfOfficeSettings": {
        "message": null,
        "isOutOfOffice": false
      }
    },
    {
      "id": "66825e03-7ef5-42da-9069-724602c31f6b",
      "availability": "Away",
      "activity": "Away",
      "outOfOfficeSettings": {
        "message": null,
        "isOutOfOffice": true
      }
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


