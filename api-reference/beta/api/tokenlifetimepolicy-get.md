---
title: Получение Токенлифетимеполици
description: Получение свойств и связей объекта Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3a45874b724ad2567caa2a60f0a43ff3dbce4955
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234507"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="bd575-103">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="bd575-103">Get tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd575-104">Получение свойств и связей объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bd575-104">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd575-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd575-105">Permissions</span></span>

<span data-ttu-id="bd575-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd575-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd575-108">Permission type</span></span>                        | <span data-ttu-id="bd575-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd575-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd575-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd575-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd575-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd575-111">Policy.Read.All</span></span> |
| <span data-ttu-id="bd575-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd575-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd575-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd575-113">Not supported.</span></span> |
| <span data-ttu-id="bd575-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd575-114">Application</span></span>                            | <span data-ttu-id="bd575-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd575-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd575-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd575-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd575-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd575-117">Optional query parameters</span></span>

<span data-ttu-id="bd575-118">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bd575-118">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="bd575-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bd575-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="bd575-120">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="bd575-120">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd575-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd575-121">Request headers</span></span>

| <span data-ttu-id="bd575-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bd575-122">Name</span></span>      |<span data-ttu-id="bd575-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bd575-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd575-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd575-124">Authorization</span></span> | <span data-ttu-id="bd575-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="bd575-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd575-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd575-126">Request body</span></span>

<span data-ttu-id="bd575-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd575-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd575-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd575-128">Response</span></span>

<span data-ttu-id="bd575-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd575-129">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd575-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd575-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd575-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd575-131">Request</span></span>

<span data-ttu-id="bd575-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd575-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="bd575-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd575-133">Response</span></span>

<span data-ttu-id="bd575-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd575-134">The following is an example of the response.</span></span>

> <span data-ttu-id="bd575-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd575-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->