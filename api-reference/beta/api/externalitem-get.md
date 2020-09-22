---
title: Получение Екстерналитем
description: Получение Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a504455b1f898d675474406e249e2637c12e1c69
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192197"
---
# <a name="get-externalitem"></a><span data-ttu-id="7ced4-103">Получение Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="7ced4-103">Get externalItem</span></span>

<span data-ttu-id="7ced4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ced4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ced4-105">Получение свойств и связей объекта [екстерналитем](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="7ced4-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="7ced4-106">Этот API предоставляется только в целях диагностики.</span><span class="sxs-lookup"><span data-stu-id="7ced4-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="7ced4-107">Он не предназначен для использования в других целях.</span><span class="sxs-lookup"><span data-stu-id="7ced4-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="7ced4-108">Повторные запросы к этому API могут привести к `429` ошибкам HTTP.</span><span class="sxs-lookup"><span data-stu-id="7ced4-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="7ced4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ced4-109">Permissions</span></span>

<span data-ttu-id="7ced4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ced4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ced4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ced4-112">Permission type</span></span>                        | <span data-ttu-id="7ced4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ced4-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ced4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ced4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ced4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ced4-115">Not supported.</span></span> |
| <span data-ttu-id="7ced4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ced4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ced4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ced4-117">Not supported.</span></span> |
| <span data-ttu-id="7ced4-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ced4-118">Application</span></span>                            | <span data-ttu-id="7ced4-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ced4-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ced4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ced4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="7ced4-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7ced4-121">Path parameters</span></span>

| <span data-ttu-id="7ced4-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ced4-122">Parameter</span></span>     | <span data-ttu-id="7ced4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7ced4-123">Type</span></span>   | <span data-ttu-id="7ced4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7ced4-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="7ced4-125">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="7ced4-125">connection-id</span></span> | <span data-ttu-id="7ced4-126">string</span><span class="sxs-lookup"><span data-stu-id="7ced4-126">string</span></span> | <span data-ttu-id="7ced4-127">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7ced4-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="7ced4-128">item-id</span><span class="sxs-lookup"><span data-stu-id="7ced4-128">item-id</span></span>       | <span data-ttu-id="7ced4-129">string</span><span class="sxs-lookup"><span data-stu-id="7ced4-129">string</span></span> | <span data-ttu-id="7ced4-130">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="7ced4-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="7ced4-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ced4-131">Optional query parameters</span></span>

<span data-ttu-id="7ced4-132">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7ced4-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ced4-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ced4-133">Request headers</span></span>

| <span data-ttu-id="7ced4-134">Имя</span><span class="sxs-lookup"><span data-stu-id="7ced4-134">Name</span></span>          | <span data-ttu-id="7ced4-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7ced4-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7ced4-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ced4-136">Authorization</span></span> | <span data-ttu-id="7ced4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ced4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ced4-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ced4-139">Request body</span></span>

<span data-ttu-id="7ced4-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ced4-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ced4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ced4-141">Response</span></span>

<span data-ttu-id="7ced4-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [екстерналитем](../resources/externalitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ced4-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ced4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="7ced4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ced4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ced4-144">Request</span></span>

<span data-ttu-id="7ced4-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ced4-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7ced4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ced4-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7ced4-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7ced4-147">The following is an example of the response.</span></span>

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
