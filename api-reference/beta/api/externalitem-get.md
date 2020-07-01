---
title: Получение Екстерналитем
description: Получение Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 0e668c6ee1d571287304e0920a4636c81cd06ca7
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45005143"
---
# <a name="get-externalitem"></a><span data-ttu-id="06df4-103">Получение Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="06df4-103">Get externalItem</span></span>

<span data-ttu-id="06df4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06df4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06df4-105">Получение свойств и связей объекта [екстерналитем](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="06df4-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="06df4-106">Этот API предоставляется только в целях диагностики.</span><span class="sxs-lookup"><span data-stu-id="06df4-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="06df4-107">Он не предназначен для использования в других целях.</span><span class="sxs-lookup"><span data-stu-id="06df4-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="06df4-108">Повторные запросы к этому API могут привести к `429` ошибкам HTTP.</span><span class="sxs-lookup"><span data-stu-id="06df4-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="06df4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06df4-109">Permissions</span></span>

<span data-ttu-id="06df4-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="06df4-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="06df4-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06df4-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06df4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06df4-112">Permission type</span></span>                        | <span data-ttu-id="06df4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06df4-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06df4-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06df4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="06df4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06df4-115">Not supported.</span></span> |
| <span data-ttu-id="06df4-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06df4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06df4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06df4-117">Not supported.</span></span> |
| <span data-ttu-id="06df4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06df4-118">Application</span></span>                            | <span data-ttu-id="06df4-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06df4-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06df4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06df4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="06df4-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="06df4-121">Path parameters</span></span>

| <span data-ttu-id="06df4-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="06df4-122">Parameter</span></span>     | <span data-ttu-id="06df4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="06df4-123">Type</span></span>   | <span data-ttu-id="06df4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="06df4-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="06df4-125">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="06df4-125">connection-id</span></span> | <span data-ttu-id="06df4-126">string</span><span class="sxs-lookup"><span data-stu-id="06df4-126">string</span></span> | <span data-ttu-id="06df4-127">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="06df4-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="06df4-128">item-id</span><span class="sxs-lookup"><span data-stu-id="06df4-128">item-id</span></span>       | <span data-ttu-id="06df4-129">string</span><span class="sxs-lookup"><span data-stu-id="06df4-129">string</span></span> | <span data-ttu-id="06df4-130">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="06df4-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="06df4-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06df4-131">Optional query parameters</span></span>

<span data-ttu-id="06df4-132">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="06df4-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06df4-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06df4-133">Request headers</span></span>

| <span data-ttu-id="06df4-134">Имя</span><span class="sxs-lookup"><span data-stu-id="06df4-134">Name</span></span>          | <span data-ttu-id="06df4-135">Описание</span><span class="sxs-lookup"><span data-stu-id="06df4-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="06df4-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06df4-136">Authorization</span></span> | <span data-ttu-id="06df4-137">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="06df4-137">Bearer {token}.</span></span> <span data-ttu-id="06df4-138">Required.</span><span class="sxs-lookup"><span data-stu-id="06df4-138">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06df4-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06df4-139">Request body</span></span>

<span data-ttu-id="06df4-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06df4-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06df4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="06df4-141">Response</span></span>

<span data-ttu-id="06df4-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [екстерналитем](../resources/externalitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06df4-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06df4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="06df4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="06df4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="06df4-144">Request</span></span>

<span data-ttu-id="06df4-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06df4-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="06df4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="06df4-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="06df4-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06df4-147">The following is an example of the response.</span></span>

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
      "identitySource": "Azure Active Directory"
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
