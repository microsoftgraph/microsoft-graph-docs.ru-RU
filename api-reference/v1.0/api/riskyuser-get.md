---
title: Получение Рискюсер
description: Чтение свойств и связей объекта Рискюсер.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb017f25388a75157a5050b0a08049b075d67ab0
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897570"
---
# <a name="get-riskyuser"></a><span data-ttu-id="3e474-103">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="3e474-103">Get riskyUser</span></span>
<span data-ttu-id="3e474-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e474-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e474-105">Чтение свойств и связей объекта [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="3e474-105">Read the properties and relationships of a [riskyUser](../resources/riskyuser.md) object.</span></span>

><span data-ttu-id="3e474-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="3e474-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e474-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e474-107">Permissions</span></span>
<span data-ttu-id="3e474-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3e474-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3e474-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="3e474-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="3e474-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e474-110">Permission type</span></span>      | <span data-ttu-id="3e474-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e474-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e474-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e474-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e474-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e474-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="3e474-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e474-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e474-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e474-115">Not supported.</span></span>    |
|<span data-ttu-id="3e474-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e474-116">Application</span></span> | <span data-ttu-id="3e474-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e474-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e474-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e474-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e474-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e474-119">Optional query parameters</span></span>
<span data-ttu-id="3e474-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e474-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3e474-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3e474-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e474-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e474-122">Request headers</span></span>
|<span data-ttu-id="3e474-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3e474-123">Name</span></span>|<span data-ttu-id="3e474-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3e474-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3e474-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e474-125">Authorization</span></span>|<span data-ttu-id="3e474-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="3e474-126">Bearer {token}.</span></span> <span data-ttu-id="3e474-127">Required.</span><span class="sxs-lookup"><span data-stu-id="3e474-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e474-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e474-128">Request body</span></span>
<span data-ttu-id="3e474-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e474-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e474-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e474-130">Response</span></span>

<span data-ttu-id="3e474-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e474-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e474-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="3e474-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e474-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e474-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```


### <a name="response"></a><span data-ttu-id="3e474-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e474-134">Response</span></span>
<span data-ttu-id="3e474-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3e474-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
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

