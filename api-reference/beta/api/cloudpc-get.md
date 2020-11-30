---
title: Получение Клаудпкс
description: Просмотр свойств и связей объекта Клаудпк.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 1fe20b9ebf70b62a1a5bb571e1b60f21c6c54acc
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378530"
---
# <a name="get-cloudpc"></a><span data-ttu-id="3604a-103">Получение Клаудпк</span><span class="sxs-lookup"><span data-stu-id="3604a-103">Get cloudPC</span></span>

<span data-ttu-id="3604a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3604a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3604a-105">Чтение свойств и связей определенного объекта [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="3604a-105">Read the properties and relationships of a specific [cloudPC](../resources/cloudpc.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3604a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3604a-106">Permissions</span></span>

<span data-ttu-id="3604a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3604a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3604a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3604a-109">Permission type</span></span>|<span data-ttu-id="3604a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3604a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3604a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3604a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3604a-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3604a-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="3604a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3604a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3604a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3604a-114">Not supported.</span></span>|
|<span data-ttu-id="3604a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3604a-115">Application</span></span>|<span data-ttu-id="3604a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3604a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3604a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3604a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3604a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3604a-118">Optional query parameters</span></span>

<span data-ttu-id="3604a-119">Этот метод поддерживает `$select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3604a-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="3604a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3604a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3604a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3604a-121">Request headers</span></span>

| <span data-ttu-id="3604a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3604a-122">Name</span></span>          | <span data-ttu-id="3604a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3604a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3604a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3604a-124">Authorization</span></span> | <span data-ttu-id="3604a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3604a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3604a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3604a-127">Request body</span></span>

<span data-ttu-id="3604a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3604a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3604a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3604a-129">Response</span></span>

<span data-ttu-id="3604a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [клаудпк](../resources/cloudpc.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3604a-130">If successful, this method returns a `200 OK` response code and a [cloudPC](../resources/cloudpc.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3604a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3604a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3604a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3604a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpc"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}
```

### <a name="response"></a><span data-ttu-id="3604a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3604a-133">Response</span></span>

<span data-ttu-id="3604a-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3604a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_cloudpc",
  "@odata.type": "microsoft.graph.cloudPC"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPC",
    "id": "ac74ae8b-85f7-4272-88cc-54192674ffff",
    "displayName": "Display Name value",
    "imageDisplayName": "Image Display Name value",
    "managedDeviceId": "e87f50c7-fa7f-4687-aade-dd45f3d6ffff",  
    "managedDeviceName": "Device Name value",
    "provisioningPolicyId": "13fa0778-ba00-438a-96d3-488c8602ffff",
    "servicePlanId": "da5615b4-a484-4742-a019-2d52c91cffff",
    "servicePlanName": "standard",
    "status": "failed",
    "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails",
    "code": "Sample code",
    "message": "Sample message",
    "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Sample value"
        }
      ]
    },
    "userPrincipalName": "User Principal Name value",
    "lastModifiedDateTime": "2020-11-03T18:14:34Z"
  }
}
```
