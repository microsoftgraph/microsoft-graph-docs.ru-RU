---
title: 'Клаудкоммуникатионс: Жетпресенцесбюсерид'
description: Получение сведений о присутствии для нескольких пользователей.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 93a782a0d46125a1f4a4a751c45d254e293c05cb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868112"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="8b16c-103">Клаудкоммуникатионс: Жетпресенцесбюсерид</span><span class="sxs-lookup"><span data-stu-id="8b16c-103">cloudCommunications: getPresencesByUserId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b16c-104">Получение сведений о [присутствии](../resources/presence.md) для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="8b16c-104">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b16c-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b16c-105">Permissions</span></span>
<span data-ttu-id="8b16c-106">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="8b16c-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="8b16c-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b16c-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b16c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b16c-108">Permission type</span></span> | <span data-ttu-id="8b16c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b16c-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="8b16c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b16c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b16c-111">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b16c-111">Presence.Read.All</span></span>                         |
| <span data-ttu-id="8b16c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b16c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b16c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b16c-113">Not Supported.</span></span>                         |
| <span data-ttu-id="8b16c-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b16c-114">Application</span></span>                            | <span data-ttu-id="8b16c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b16c-115">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8b16c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b16c-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="8b16c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b16c-117">Request Headers</span></span>
| <span data-ttu-id="8b16c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8b16c-118">Name</span></span>          | <span data-ttu-id="8b16c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8b16c-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8b16c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b16c-120">Authorization</span></span> | <span data-ttu-id="8b16c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b16c-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8b16c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b16c-123">Content-type</span></span> | <span data-ttu-id="8b16c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b16c-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8b16c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b16c-126">Request body</span></span>

<span data-ttu-id="8b16c-127">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="8b16c-127">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="8b16c-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b16c-128">Parameter</span></span>      | <span data-ttu-id="8b16c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8b16c-129">Type</span></span>    |<span data-ttu-id="8b16c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8b16c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b16c-131">ids</span><span class="sxs-lookup"><span data-stu-id="8b16c-131">ids</span></span>|<span data-ttu-id="8b16c-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8b16c-132">String collection</span></span>|<span data-ttu-id="8b16c-133">Идентификаторы объектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b16c-133">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="8b16c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b16c-134">Response</span></span>

<span data-ttu-id="8b16c-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b16c-135">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="8b16c-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b16c-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b16c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b16c-137">Request</span></span>
<span data-ttu-id="8b16c-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b16c-138">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8b16c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b16c-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8b16c-140">C#</span><span class="sxs-lookup"><span data-stu-id="8b16c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b16c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b16c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8b16c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b16c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8b16c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b16c-143">Response</span></span>
<span data-ttu-id="8b16c-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b16c-144">The following example shows the response.</span></span>

> <span data-ttu-id="8b16c-145">**Примечание:** Объекты ответа могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8b16c-145">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="8b16c-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b16c-146">All the properties will be returned from an actual call.</span></span>

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
