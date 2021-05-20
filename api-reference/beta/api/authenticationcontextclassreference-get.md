---
title: Проверка подлинностиContextClassReference
description: Извлечение свойств и связей объекта authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3ca46a2dfff70ed32bc2e960b4f16cdca9ab7da8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547425"
---
# <a name="get-authenticationcontextclassreference"></a><span data-ttu-id="3faa3-103">Проверка подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3faa3-103">Get authenticationContextClassReference</span></span>

<span data-ttu-id="3faa3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3faa3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3faa3-105">Извлечение свойств и связей объекта [authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="3faa3-105">Retrieve the properties and relationships of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3faa3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3faa3-106">Permissions</span></span>

<span data-ttu-id="3faa3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3faa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3faa3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3faa3-109">Permission type</span></span>                        | <span data-ttu-id="3faa3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3faa3-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="3faa3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3faa3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3faa3-112">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="3faa3-112">Policy.Read.ConditionalAccess</span></span> |
|<span data-ttu-id="3faa3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3faa3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3faa3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3faa3-114">Not supported.</span></span> |
|<span data-ttu-id="3faa3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3faa3-115">Application</span></span>                            | <span data-ttu-id="3faa3-116">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="3faa3-116">Policy.Read.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="3faa3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3faa3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3faa3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3faa3-118">Optional query parameters</span></span>

<span data-ttu-id="3faa3-119">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3faa3-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3faa3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3faa3-120">Request headers</span></span>

| <span data-ttu-id="3faa3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3faa3-121">Name</span></span>      |<span data-ttu-id="3faa3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3faa3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3faa3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3faa3-123">Authorization</span></span> | <span data-ttu-id="3faa3-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3faa3-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3faa3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3faa3-125">Request body</span></span>

<span data-ttu-id="3faa3-126">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3faa3-126">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="3faa3-127">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3faa3-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="response"></a><span data-ttu-id="3faa3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3faa3-128">Response</span></span>

<span data-ttu-id="3faa3-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемую проверку `200 OK` [подлинностиContextClassReferences](../resources/\authenticationcontextclassreference.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3faa3-129">If successful, this method returns a `200 OK` response code and the requested [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3faa3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3faa3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3faa3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3faa3-131">Request</span></span>

<span data-ttu-id="3faa3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3faa3-132">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
```



### <a name="response"></a><span data-ttu-id="3faa3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3faa3-133">Response</span></span>

<span data-ttu-id="3faa3-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3faa3-134">The following is an example of the response.</span></span>

> <span data-ttu-id="3faa3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3faa3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReferences/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": false
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
