---
title: Get externalItem
description: Получите externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2c0bdc7d44e2d9fb5c317ab2eb1cbc71cca76031
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366756"
---
# <a name="get-externalitem"></a><span data-ttu-id="699b7-103">Get externalItem</span><span class="sxs-lookup"><span data-stu-id="699b7-103">Get externalItem</span></span>

<span data-ttu-id="699b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="699b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="699b7-105">Получите свойства и связи объекта [externalitem.](../resources/externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="699b7-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="699b7-106">Этот API предоставляется только для диагностических целей.</span><span class="sxs-lookup"><span data-stu-id="699b7-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="699b7-107">Она не предназначена для использования для каких-либо других целей.</span><span class="sxs-lookup"><span data-stu-id="699b7-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="699b7-108">Повторные запросы на этот API могут привести к `429` ошибкам HTTP.</span><span class="sxs-lookup"><span data-stu-id="699b7-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="699b7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="699b7-109">Permissions</span></span>

<span data-ttu-id="699b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="699b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="699b7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="699b7-112">Permission type</span></span>                        | <span data-ttu-id="699b7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="699b7-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="699b7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="699b7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="699b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="699b7-115">Not supported.</span></span> |
| <span data-ttu-id="699b7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="699b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="699b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="699b7-117">Not supported.</span></span> |
| <span data-ttu-id="699b7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="699b7-118">Application</span></span>                            | <span data-ttu-id="699b7-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="699b7-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="699b7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="699b7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="699b7-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="699b7-121">Path parameters</span></span>

| <span data-ttu-id="699b7-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="699b7-122">Parameter</span></span>     | <span data-ttu-id="699b7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="699b7-123">Type</span></span>   | <span data-ttu-id="699b7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="699b7-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="699b7-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="699b7-125">connection-id</span></span> | <span data-ttu-id="699b7-126">string</span><span class="sxs-lookup"><span data-stu-id="699b7-126">string</span></span> | <span data-ttu-id="699b7-127">`id`Свойствосодержащего [externalConnection](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="699b7-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="699b7-128">item-id</span><span class="sxs-lookup"><span data-stu-id="699b7-128">item-id</span></span>       | <span data-ttu-id="699b7-129">string</span><span class="sxs-lookup"><span data-stu-id="699b7-129">string</span></span> | <span data-ttu-id="699b7-130">Свойство `id` [externalItem,](../resources/externalitem.md)предоставленное разработчиком.</span><span class="sxs-lookup"><span data-stu-id="699b7-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="699b7-131">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="699b7-131">Optional query parameters</span></span>

<span data-ttu-id="699b7-132">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="699b7-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="699b7-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="699b7-133">Request headers</span></span>

| <span data-ttu-id="699b7-134">Имя</span><span class="sxs-lookup"><span data-stu-id="699b7-134">Name</span></span>          | <span data-ttu-id="699b7-135">Описание</span><span class="sxs-lookup"><span data-stu-id="699b7-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="699b7-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="699b7-136">Authorization</span></span> | <span data-ttu-id="699b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="699b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="699b7-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="699b7-139">Request body</span></span>

<span data-ttu-id="699b7-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="699b7-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="699b7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="699b7-141">Response</span></span>

<span data-ttu-id="699b7-142">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект externalItem](../resources/externalitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="699b7-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="699b7-143">Пример</span><span class="sxs-lookup"><span data-stu-id="699b7-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="699b7-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="699b7-144">Request</span></span>

<span data-ttu-id="699b7-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="699b7-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="699b7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="699b7-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="699b7-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="699b7-147">The following is an example of the response.</span></span>

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
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    },
    {
      "type": "group",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
      "identitySource": "external"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
