---
title: 'cloudCommunications: getPresencesByUserId'
description: Получите сведения о присутствии для нескольких пользователей.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 78793623972e5887a1f74184789dbda87ee4dda4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964014"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="30e43-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="30e43-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="30e43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30e43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30e43-105">Получите сведения [о](../resources/presence.md) присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="30e43-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="30e43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30e43-106">Permissions</span></span>
<span data-ttu-id="30e43-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="30e43-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="30e43-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e43-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30e43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30e43-109">Permission type</span></span> | <span data-ttu-id="30e43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30e43-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="30e43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30e43-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="30e43-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e43-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="30e43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30e43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e43-114">Not Supported.</span></span>                         |
| <span data-ttu-id="30e43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30e43-115">Application</span></span>                            | <span data-ttu-id="30e43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e43-116">Not Supported.</span></span>                                  |

> <span data-ttu-id="30e43-117">**Примечание:**</span><span class="sxs-lookup"><span data-stu-id="30e43-117">**Note:**</span></span>
> * <span data-ttu-id="30e43-118">В запросе API поддерживается не более 650 пользовательских ИД.</span><span class="sxs-lookup"><span data-stu-id="30e43-118">Maximum of 650 user IDs are supported per API request.</span></span>
> * <span data-ttu-id="30e43-119">Максимальная скорость запроса этого API — 1500 запросов API в течение 30 секунд на каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="30e43-119">The maximum request rate of this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="30e43-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30e43-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="30e43-121">Запрашивать заглавные</span><span class="sxs-lookup"><span data-stu-id="30e43-121">Request Headers</span></span>
| <span data-ttu-id="30e43-122">Имя</span><span class="sxs-lookup"><span data-stu-id="30e43-122">Name</span></span>          | <span data-ttu-id="30e43-123">Описание</span><span class="sxs-lookup"><span data-stu-id="30e43-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="30e43-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30e43-124">Authorization</span></span> | <span data-ttu-id="30e43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30e43-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="30e43-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30e43-127">Content-type</span></span> | <span data-ttu-id="30e43-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30e43-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="30e43-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30e43-130">Request body</span></span>

<span data-ttu-id="30e43-131">В теле запроса укажи объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="30e43-131">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="30e43-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="30e43-132">Parameter</span></span>      | <span data-ttu-id="30e43-133">Тип</span><span class="sxs-lookup"><span data-stu-id="30e43-133">Type</span></span>    |<span data-ttu-id="30e43-134">Описание</span><span class="sxs-lookup"><span data-stu-id="30e43-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30e43-135">ids</span><span class="sxs-lookup"><span data-stu-id="30e43-135">ids</span></span>|<span data-ttu-id="30e43-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="30e43-136">String collection</span></span>|<span data-ttu-id="30e43-137">ID объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="30e43-137">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="30e43-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="30e43-138">Response</span></span>

<span data-ttu-id="30e43-139">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` присутствия в тексте ответа. [](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="30e43-139">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="30e43-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="30e43-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30e43-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="30e43-141">Request</span></span>
<span data-ttu-id="30e43-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30e43-142">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="30e43-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="30e43-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[<span data-ttu-id="30e43-144">C#</span><span class="sxs-lookup"><span data-stu-id="30e43-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30e43-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30e43-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30e43-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30e43-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30e43-147">Java</span><span class="sxs-lookup"><span data-stu-id="30e43-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="30e43-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="30e43-148">Response</span></span>
<span data-ttu-id="30e43-149">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30e43-149">The following example shows the response.</span></span>

> <span data-ttu-id="30e43-150">**Примечание:** Объекты отклика могут быть сокращены для читаемости.</span><span class="sxs-lookup"><span data-stu-id="30e43-150">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="30e43-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30e43-151">All the properties will be returned from an actual call.</span></span>

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


