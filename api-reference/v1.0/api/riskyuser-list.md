---
title: Список riskyUsers
description: Получите список объектов riskyUser и их свойств.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc72c174b81a5d2442b264026305e28cbb03afdf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448062"
---
# <a name="list-riskyusers"></a><span data-ttu-id="ee1e3-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ee1e3-103">List riskyUsers</span></span>
<span data-ttu-id="ee1e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee1e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee1e3-105">Получите список объектов [riskyUser](../resources/riskyuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee1e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee1e3-106">Permissions</span></span>
<span data-ttu-id="ee1e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="ee1e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="ee1e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee1e3-109">Permission type</span></span>|<span data-ttu-id="ee1e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee1e3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee1e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee1e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee1e3-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee1e3-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="ee1e3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee1e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee1e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-114">Not supported.</span></span>    |
|<span data-ttu-id="ee1e3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee1e3-115">Application</span></span> | <span data-ttu-id="ee1e3-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee1e3-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee1e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee1e3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee1e3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee1e3-118">Optional query parameters</span></span>
<span data-ttu-id="ee1e3-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee1e3-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ee1e3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee1e3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee1e3-121">Request headers</span></span>
|<span data-ttu-id="ee1e3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ee1e3-122">Name</span></span>|<span data-ttu-id="ee1e3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ee1e3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee1e3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee1e3-124">Authorization</span></span>|<span data-ttu-id="ee1e3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee1e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee1e3-127">Request body</span></span>
<span data-ttu-id="ee1e3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee1e3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee1e3-129">Response</span></span>

<span data-ttu-id="ee1e3-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [riskyUser](../resources/riskyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee1e3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ee1e3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee1e3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee1e3-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="ee1e3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee1e3-133">Response</span></span>
<span data-ttu-id="ee1e3-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee1e3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUser",
      "id": "d1d4a5d4-a5d4-d1d4-d4a5-d4d1d4a5d4d1",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String"
    }
  ]
}
```


