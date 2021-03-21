---
title: Список riskyUsers
description: Получите список объектов riskyUser и их свойств.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c0e47c6de003bdb24cea59bc0f36e76db4e68472
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958229"
---
# <a name="list-riskyusers"></a><span data-ttu-id="7be48-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7be48-103">List riskyUsers</span></span>
<span data-ttu-id="7be48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7be48-105">Получите список объектов [riskyUser](../resources/riskyuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="7be48-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7be48-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7be48-106">Permissions</span></span>
<span data-ttu-id="7be48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7be48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="7be48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7be48-109">Permission type</span></span>|<span data-ttu-id="7be48-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7be48-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7be48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7be48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7be48-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7be48-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="7be48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7be48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7be48-114">Not supported.</span></span>    |
|<span data-ttu-id="7be48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7be48-115">Application</span></span> | <span data-ttu-id="7be48-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7be48-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7be48-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7be48-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7be48-118">Optional query parameters</span></span>
<span data-ttu-id="7be48-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7be48-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7be48-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7be48-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7be48-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7be48-121">Request headers</span></span>
|<span data-ttu-id="7be48-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7be48-122">Name</span></span>|<span data-ttu-id="7be48-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7be48-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7be48-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7be48-124">Authorization</span></span>|<span data-ttu-id="7be48-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7be48-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7be48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7be48-127">Request body</span></span>
<span data-ttu-id="7be48-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7be48-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7be48-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7be48-129">Response</span></span>

<span data-ttu-id="7be48-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [riskyUser](../resources/riskyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7be48-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7be48-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7be48-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7be48-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7be48-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="7be48-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7be48-133">Response</span></span>
<span data-ttu-id="7be48-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7be48-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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


