---
title: Список Клаудпкс
description: Список свойств и связей объектов Клаудпк.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: cb7b5e79d3fd490fc574fbfbb8c08988321bc86d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378599"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="8ae72-103">Список Клаудпкс</span><span class="sxs-lookup"><span data-stu-id="8ae72-103">List cloudPCs</span></span>

<span data-ttu-id="8ae72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ae72-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ae72-105">Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="8ae72-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ae72-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ae72-106">Permissions</span></span>

<span data-ttu-id="8ae72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae72-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ae72-109">Permission type</span></span>|<span data-ttu-id="8ae72-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ae72-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae72-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ae72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ae72-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8ae72-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="8ae72-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ae72-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae72-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae72-114">Not supported.</span></span>|
|<span data-ttu-id="8ae72-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ae72-115">Application</span></span>|<span data-ttu-id="8ae72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae72-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae72-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ae72-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ae72-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8ae72-118">Optional query parameters</span></span>

<span data-ttu-id="8ae72-119">Этот метод поддерживает `$select` `$filter` и `$count` параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8ae72-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8ae72-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8ae72-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ae72-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ae72-121">Request headers</span></span>

| <span data-ttu-id="8ae72-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8ae72-122">Name</span></span>          | <span data-ttu-id="8ae72-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae72-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8ae72-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ae72-124">Authorization</span></span> | <span data-ttu-id="8ae72-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ae72-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ae72-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ae72-127">Request body</span></span>

<span data-ttu-id="8ae72-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ae72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ae72-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ae72-129">Response</span></span>

<span data-ttu-id="8ae72-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаудпк](../resources/cloudpc.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ae72-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ae72-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ae72-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ae72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ae72-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```

### <a name="response"></a><span data-ttu-id="8ae72-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ae72-133">Response</span></span>

<span data-ttu-id="8ae72-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8ae72-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPC)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPC",
      "id": "662009bc-7732-4f6f-8726-25883518ffff",
      "displayName": "Display Name value",
      "imageDisplayName": "Image Display Name value",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "Managed Device Name value",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "User Principal Name value",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null
    }
  ]
}
```
