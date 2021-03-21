---
title: Get riskyUser
description: Ознакомьтесь с свойствами и отношениями объекта riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fac6527f330bfc6f45e3a6acc773ac4323fcea75
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959454"
---
# <a name="get-riskyuser"></a><span data-ttu-id="0ad1e-103">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="0ad1e-103">Get riskyUser</span></span>
<span data-ttu-id="0ad1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ad1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ad1e-105">Ознакомьтесь с свойствами и отношениями объекта [riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="0ad1e-105">Read the properties and relationships of a [riskyUser](../resources/riskyuser.md) object.</span></span>

><span data-ttu-id="0ad1e-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ad1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ad1e-107">Permissions</span></span>
<span data-ttu-id="0ad1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="0ad1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="0ad1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ad1e-110">Permission type</span></span>      | <span data-ttu-id="0ad1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ad1e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ad1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ad1e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ad1e-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ad1e-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="0ad1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ad1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ad1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-115">Not supported.</span></span>    |
|<span data-ttu-id="0ad1e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ad1e-116">Application</span></span> | <span data-ttu-id="0ad1e-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ad1e-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ad1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ad1e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ad1e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ad1e-119">Optional query parameters</span></span>
<span data-ttu-id="0ad1e-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0ad1e-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0ad1e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ad1e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ad1e-122">Request headers</span></span>
|<span data-ttu-id="0ad1e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0ad1e-123">Name</span></span>|<span data-ttu-id="0ad1e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0ad1e-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ad1e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ad1e-125">Authorization</span></span>|<span data-ttu-id="0ad1e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ad1e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ad1e-128">Request body</span></span>
<span data-ttu-id="0ad1e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ad1e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ad1e-130">Response</span></span>

<span data-ttu-id="0ad1e-131">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [riskyUser](../resources/riskyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ad1e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ad1e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ad1e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ad1e-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```


### <a name="response"></a><span data-ttu-id="0ad1e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ad1e-134">Response</span></span>
<span data-ttu-id="0ad1e-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ad1e-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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


