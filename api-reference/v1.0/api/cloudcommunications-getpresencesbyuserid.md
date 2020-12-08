---
title: 'Клаудкоммуникатионс: Жетпресенцесбюсерид'
description: Получение сведений о присутствии для нескольких пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: e06c1403b1d96a42a670f4c6d53c3bf5251d3b8a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581238"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="04b8e-103">Клаудкоммуникатионс: Жетпресенцесбюсерид</span><span class="sxs-lookup"><span data-stu-id="04b8e-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="04b8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04b8e-105">Получение сведений о [присутствии](../resources/presence.md) для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="04b8e-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="04b8e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="04b8e-106">Permissions</span></span>
<span data-ttu-id="04b8e-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="04b8e-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="04b8e-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b8e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04b8e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b8e-109">Permission type</span></span> | <span data-ttu-id="04b8e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b8e-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="04b8e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b8e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04b8e-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b8e-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="04b8e-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b8e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b8e-114">Not Supported.</span></span>                         |
| <span data-ttu-id="04b8e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="04b8e-115">Application</span></span>                            | <span data-ttu-id="04b8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b8e-116">Not Supported.</span></span>                                  |

> <span data-ttu-id="04b8e-117">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="04b8e-117">**Note:**</span></span>
> * <span data-ttu-id="04b8e-118">Для каждого запроса API поддерживается не более 650 идентификаторов пользователей.</span><span class="sxs-lookup"><span data-stu-id="04b8e-118">Maximum of 650 user IDs are supported per API request.</span></span>
> * <span data-ttu-id="04b8e-119">Максимальная частота запросов для этого API составляет 1500 запросов API в течение 30-секундного периода на приложение для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="04b8e-119">The maximum request rate of this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="04b8e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b8e-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="04b8e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b8e-121">Request Headers</span></span>
| <span data-ttu-id="04b8e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="04b8e-122">Name</span></span>          | <span data-ttu-id="04b8e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="04b8e-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="04b8e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b8e-124">Authorization</span></span> | <span data-ttu-id="04b8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b8e-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="04b8e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04b8e-127">Content-type</span></span> | <span data-ttu-id="04b8e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b8e-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="04b8e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b8e-130">Request body</span></span>

<span data-ttu-id="04b8e-131">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="04b8e-131">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="04b8e-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="04b8e-132">Parameter</span></span>      | <span data-ttu-id="04b8e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="04b8e-133">Type</span></span>    |<span data-ttu-id="04b8e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="04b8e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04b8e-135">ids</span><span class="sxs-lookup"><span data-stu-id="04b8e-135">ids</span></span>|<span data-ttu-id="04b8e-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04b8e-136">String collection</span></span>|<span data-ttu-id="04b8e-137">Идентификаторы объектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="04b8e-137">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="04b8e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b8e-138">Response</span></span>

<span data-ttu-id="04b8e-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04b8e-139">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="04b8e-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="04b8e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04b8e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b8e-141">Request</span></span>
<span data-ttu-id="04b8e-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b8e-142">The following example shows a request.</span></span>

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

---

### <a name="response"></a><span data-ttu-id="04b8e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b8e-143">Response</span></span>
<span data-ttu-id="04b8e-144">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04b8e-144">The following example shows the response.</span></span>

> <span data-ttu-id="04b8e-145">**Примечание:** Объекты ответа могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04b8e-145">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="04b8e-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04b8e-146">All the properties will be returned from an actual call.</span></span>

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


