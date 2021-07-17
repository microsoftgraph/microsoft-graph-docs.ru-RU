---
title: Get externalItem
description: Ознакомьтесь с свойствами и отношениями объекта externalItem.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6defb4476d5d34b148e8e18c4757333f9bc3ca81
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467497"
---
# <a name="get-externalitem"></a><span data-ttu-id="79c56-103">Get externalItem</span><span class="sxs-lookup"><span data-stu-id="79c56-103">Get externalItem</span></span>
<span data-ttu-id="79c56-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="79c56-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="79c56-105">Ознакомьтесь с свойствами и отношениями [объекта externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="79c56-105">Read the properties and relationships of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79c56-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79c56-106">Permissions</span></span>
<span data-ttu-id="79c56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79c56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79c56-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79c56-109">Permission type</span></span>|<span data-ttu-id="79c56-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79c56-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79c56-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79c56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79c56-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="79c56-112">Not applicable</span></span>|
|<span data-ttu-id="79c56-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79c56-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79c56-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="79c56-114">Not applicable</span></span>|
|<span data-ttu-id="79c56-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="79c56-115">Application</span></span>| <span data-ttu-id="79c56-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79c56-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79c56-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79c56-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/items/{externalItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79c56-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79c56-118">Optional query parameters</span></span>
<span data-ttu-id="79c56-119">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="79c56-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79c56-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79c56-120">Request headers</span></span>
|<span data-ttu-id="79c56-121">Имя</span><span class="sxs-lookup"><span data-stu-id="79c56-121">Name</span></span>|<span data-ttu-id="79c56-122">Описание</span><span class="sxs-lookup"><span data-stu-id="79c56-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79c56-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79c56-123">Authorization</span></span>|<span data-ttu-id="79c56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79c56-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79c56-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79c56-126">Request body</span></span>
<span data-ttu-id="79c56-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79c56-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79c56-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c56-128">Response</span></span>

<span data-ttu-id="79c56-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект externalItem](../resources/externalconnectors-externalitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="79c56-129">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalconnectors-externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79c56-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="79c56-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79c56-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="79c56-131">Request</span></span>
<span data-ttu-id="79c56-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79c56-132">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```


### <a name="response"></a><span data-ttu-id="79c56-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c56-133">Response</span></span>
<span data-ttu-id="79c56-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79c56-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```

