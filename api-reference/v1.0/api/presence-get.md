---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a82c03e9b63d83f8aab8b3556e75b17d926ff3e6
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581249"
---
# <a name="get-presence"></a><span data-ttu-id="7e83c-103">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="7e83c-103">Get presence</span></span>

<span data-ttu-id="7e83c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e83c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e83c-105">Получение сведений о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e83c-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e83c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e83c-106">Permissions</span></span>
<span data-ttu-id="7e83c-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="7e83c-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="7e83c-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e83c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e83c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e83c-109">Permission type</span></span> | <span data-ttu-id="7e83c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e83c-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="7e83c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e83c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e83c-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e83c-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="7e83c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e83c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e83c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e83c-114">Not Supported.</span></span>                        |
| <span data-ttu-id="7e83c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e83c-115">Application</span></span>                            | <span data-ttu-id="7e83c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e83c-116">Not Supported.</span></span>                        |

> <span data-ttu-id="7e83c-117">**Примечание:** Максимальная частота запросов для этого API составляет 1500 запросов API в течение 30-секундного периода на приложение для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="7e83c-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="7e83c-118">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="7e83c-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="7e83c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e83c-119">Request Headers</span></span>
| <span data-ttu-id="7e83c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7e83c-120">Name</span></span>          | <span data-ttu-id="7e83c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7e83c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7e83c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e83c-122">Authorization</span></span> | <span data-ttu-id="7e83c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e83c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="7e83c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e83c-125">Request body</span></span>

<span data-ttu-id="7e83c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e83c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e83c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e83c-127">Response</span></span>
<span data-ttu-id="7e83c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [присутствия](../resources/presence.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e83c-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e83c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e83c-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="7e83c-130">Пример 1: получение собственных сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="7e83c-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="7e83c-131">В приведенном ниже примере показано, как получить сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="7e83c-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="7e83c-132">Для выполнения этой операции требуется разрешение на присутствие. чтение.</span><span class="sxs-lookup"><span data-stu-id="7e83c-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="7e83c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e83c-133">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```

---


#### <a name="response"></a><span data-ttu-id="7e83c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e83c-134">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="7e83c-135">Пример 2: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="7e83c-135">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="7e83c-136">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e83c-136">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="7e83c-137">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="7e83c-137">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="7e83c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e83c-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

---


#### <a name="response"></a><span data-ttu-id="7e83c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e83c-139">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="7e83c-140">Пример 3: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="7e83c-140">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="7e83c-141">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e83c-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="7e83c-142">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="7e83c-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="7e83c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e83c-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a><span data-ttu-id="7e83c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e83c-144">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


