---
title: Получение Екстерналитем
description: Получение Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a894afa05207dc483e5fbbf3e4de14e0b400f894
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006808"
---
# <a name="get-externalitem"></a><span data-ttu-id="3d114-103">Получение Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="3d114-103">Get externalItem</span></span>

<span data-ttu-id="3d114-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d114-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d114-105">Получение свойств и связей объекта [екстерналитем](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3d114-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="3d114-106">Этот API предоставляется только в целях диагностики.</span><span class="sxs-lookup"><span data-stu-id="3d114-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="3d114-107">Он не предназначен для использования в других целях.</span><span class="sxs-lookup"><span data-stu-id="3d114-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="3d114-108">Повторные запросы к этому API могут привести к `429` ошибкам HTTP.</span><span class="sxs-lookup"><span data-stu-id="3d114-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="3d114-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d114-109">Permissions</span></span>

<span data-ttu-id="3d114-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d114-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d114-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d114-112">Permission type</span></span>                        | <span data-ttu-id="3d114-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d114-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d114-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d114-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d114-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d114-115">Not supported.</span></span> |
| <span data-ttu-id="3d114-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d114-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d114-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d114-117">Not supported.</span></span> |
| <span data-ttu-id="3d114-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d114-118">Application</span></span>                            | <span data-ttu-id="3d114-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d114-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d114-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d114-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="3d114-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3d114-121">Path parameters</span></span>

| <span data-ttu-id="3d114-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="3d114-122">Parameter</span></span>     | <span data-ttu-id="3d114-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3d114-123">Type</span></span>   | <span data-ttu-id="3d114-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3d114-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="3d114-125">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="3d114-125">connection-id</span></span> | <span data-ttu-id="3d114-126">string</span><span class="sxs-lookup"><span data-stu-id="3d114-126">string</span></span> | <span data-ttu-id="3d114-127">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="3d114-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="3d114-128">item-id</span><span class="sxs-lookup"><span data-stu-id="3d114-128">item-id</span></span>       | <span data-ttu-id="3d114-129">string</span><span class="sxs-lookup"><span data-stu-id="3d114-129">string</span></span> | <span data-ttu-id="3d114-130">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="3d114-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3d114-131">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3d114-131">Optional query parameters</span></span>

<span data-ttu-id="3d114-132">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3d114-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d114-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d114-133">Request headers</span></span>

| <span data-ttu-id="3d114-134">Имя</span><span class="sxs-lookup"><span data-stu-id="3d114-134">Name</span></span>          | <span data-ttu-id="3d114-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3d114-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3d114-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d114-136">Authorization</span></span> | <span data-ttu-id="3d114-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d114-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d114-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d114-139">Request body</span></span>

<span data-ttu-id="3d114-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d114-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d114-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d114-141">Response</span></span>

<span data-ttu-id="3d114-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [екстерналитем](../resources/externalitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d114-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d114-143">Пример</span><span class="sxs-lookup"><span data-stu-id="3d114-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d114-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d114-144">Request</span></span>

<span data-ttu-id="3d114-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d114-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="3d114-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d114-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="3d114-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3d114-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


