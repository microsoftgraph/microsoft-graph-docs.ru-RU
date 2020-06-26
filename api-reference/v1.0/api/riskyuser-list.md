---
title: Список riskyUsers
description: Получение списка объектов Рискюсер и их свойств.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd6d413803e7461ffe0f00891b6e4db7cd3d0e0b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897556"
---
# <a name="list-riskyusers"></a><span data-ttu-id="69c40-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="69c40-103">List riskyUsers</span></span>
<span data-ttu-id="69c40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69c40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69c40-105">Получение списка объектов [рискюсер](../resources/riskyuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="69c40-105">Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="69c40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69c40-106">Permissions</span></span>
<span data-ttu-id="69c40-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="69c40-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="69c40-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="69c40-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="69c40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69c40-109">Permission type</span></span>|<span data-ttu-id="69c40-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69c40-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69c40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69c40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69c40-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="69c40-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="69c40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69c40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69c40-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69c40-114">Not supported.</span></span>    |
|<span data-ttu-id="69c40-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="69c40-115">Application</span></span> | <span data-ttu-id="69c40-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="69c40-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69c40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69c40-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69c40-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69c40-118">Optional query parameters</span></span>
<span data-ttu-id="69c40-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="69c40-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="69c40-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="69c40-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="69c40-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69c40-121">Request headers</span></span>
|<span data-ttu-id="69c40-122">Имя</span><span class="sxs-lookup"><span data-stu-id="69c40-122">Name</span></span>|<span data-ttu-id="69c40-123">Описание</span><span class="sxs-lookup"><span data-stu-id="69c40-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69c40-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69c40-124">Authorization</span></span>|<span data-ttu-id="69c40-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="69c40-125">Bearer {token}.</span></span> <span data-ttu-id="69c40-126">Required.</span><span class="sxs-lookup"><span data-stu-id="69c40-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69c40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69c40-127">Request body</span></span>
<span data-ttu-id="69c40-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69c40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69c40-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="69c40-129">Response</span></span>

<span data-ttu-id="69c40-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69c40-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69c40-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="69c40-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69c40-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="69c40-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers
```


### <a name="response"></a><span data-ttu-id="69c40-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="69c40-133">Response</span></span>
<span data-ttu-id="69c40-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="69c40-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

