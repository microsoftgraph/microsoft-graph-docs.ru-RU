---
title: Список Клаудпкпровисионингполици
description: Просмотр свойств и связей всех политик подготовки облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b9d62152228518aa856b48e3fc064ce77fd1801f
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378590"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="8db6a-103">Список ПровисионингполиЦиес</span><span class="sxs-lookup"><span data-stu-id="8db6a-103">List provisioningPolicies</span></span>

<span data-ttu-id="8db6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8db6a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8db6a-105">Список свойств и связей объектов [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8db6a-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8db6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8db6a-106">Permissions</span></span>

<span data-ttu-id="8db6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8db6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8db6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8db6a-109">Permission type</span></span>|<span data-ttu-id="8db6a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8db6a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8db6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8db6a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8db6a-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8db6a-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="8db6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8db6a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8db6a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8db6a-114">Not supported.</span></span>|
|<span data-ttu-id="8db6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8db6a-115">Application</span></span>|<span data-ttu-id="8db6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8db6a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8db6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8db6a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8db6a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8db6a-118">Optional query parameters</span></span>

<span data-ttu-id="8db6a-119">Этот метод поддерживает `$select` `$filter` и `$expand` параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8db6a-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8db6a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8db6a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8db6a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8db6a-121">Request headers</span></span>

| <span data-ttu-id="8db6a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8db6a-122">Name</span></span>          | <span data-ttu-id="8db6a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8db6a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8db6a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8db6a-124">Authorization</span></span> | <span data-ttu-id="8db6a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8db6a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8db6a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8db6a-127">Request body</span></span>

<span data-ttu-id="8db6a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8db6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8db6a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8db6a-129">Response</span></span>

<span data-ttu-id="8db6a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8db6a-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8db6a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8db6a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8db6a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8db6a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```

### <a name="response"></a><span data-ttu-id="8db6a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8db6a-133">Response</span></span>

<span data-ttu-id="8db6a-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8db6a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcProvisioningPolicy)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
      "id": "1d164206-bf41-4fd2-8424-a3192d392273",
      "displayName": "Display Name value",
      "description": "Description value",
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "imageId": "Image ID value",
      "imageDisplayName": "Image Display Name value",
      "imageType":"custom"
    }
  ]
}
```
