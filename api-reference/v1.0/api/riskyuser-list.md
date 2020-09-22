---
title: Список riskyUsers
description: Получение списка объектов Рискюсер и их свойств.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef4816819e82944e752fb47fdc63a88f7f8a29a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051328"
---
# <a name="list-riskyusers"></a><span data-ttu-id="98a7f-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="98a7f-103">List riskyUsers</span></span>
<span data-ttu-id="98a7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98a7f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98a7f-105">Получение списка объектов [рискюсер](../resources/riskyuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="98a7f-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="98a7f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98a7f-106">Permissions</span></span>
<span data-ttu-id="98a7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="98a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="98a7f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98a7f-109">Permission type</span></span>|<span data-ttu-id="98a7f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98a7f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98a7f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98a7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="98a7f-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="98a7f-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="98a7f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98a7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98a7f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98a7f-114">Not supported.</span></span>    |
|<span data-ttu-id="98a7f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98a7f-115">Application</span></span> | <span data-ttu-id="98a7f-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="98a7f-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98a7f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98a7f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98a7f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98a7f-118">Optional query parameters</span></span>
<span data-ttu-id="98a7f-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="98a7f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="98a7f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="98a7f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="98a7f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98a7f-121">Request headers</span></span>
|<span data-ttu-id="98a7f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="98a7f-122">Name</span></span>|<span data-ttu-id="98a7f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="98a7f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="98a7f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98a7f-124">Authorization</span></span>|<span data-ttu-id="98a7f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98a7f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98a7f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98a7f-127">Request body</span></span>
<span data-ttu-id="98a7f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98a7f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98a7f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="98a7f-129">Response</span></span>

<span data-ttu-id="98a7f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98a7f-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98a7f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="98a7f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98a7f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98a7f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="98a7f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="98a7f-133">Response</span></span>
<span data-ttu-id="98a7f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98a7f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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


