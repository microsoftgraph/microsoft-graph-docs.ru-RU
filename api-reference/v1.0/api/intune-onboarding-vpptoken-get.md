---
title: Получить vppToken
description: Чтение свойств и связей объекта vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11d1346bc28edc057f77df0854496c84813add96
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759053"
---
# <a name="get-vpptoken"></a><span data-ttu-id="fc1fe-103">Получить vppToken</span><span class="sxs-lookup"><span data-stu-id="fc1fe-103">Get vppToken</span></span>

<span data-ttu-id="fc1fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc1fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc1fe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc1fe-106">Чтение свойств и связей объекта [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="fc1fe-106">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc1fe-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="fc1fe-107">Prerequisites</span></span>
<span data-ttu-id="fc1fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc1fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc1fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc1fe-110">Permission type</span></span>|<span data-ttu-id="fc1fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc1fe-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc1fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc1fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc1fe-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc1fe-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc1fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc1fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc1fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-115">Not supported.</span></span>|
|<span data-ttu-id="fc1fe-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fc1fe-116">Application</span></span>|<span data-ttu-id="fc1fe-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc1fe-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc1fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc1fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc1fe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc1fe-119">Optional query parameters</span></span>
<span data-ttu-id="fc1fe-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc1fe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc1fe-121">Request headers</span></span>
|<span data-ttu-id="fc1fe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc1fe-122">Header</span></span>|<span data-ttu-id="fc1fe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fc1fe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc1fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc1fe-124">Authorization</span></span>|<span data-ttu-id="fc1fe-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc1fe-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fc1fe-126">Accept</span></span>|<span data-ttu-id="fc1fe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fc1fe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc1fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc1fe-128">Request body</span></span>
<span data-ttu-id="fc1fe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc1fe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc1fe-130">Response</span></span>
<span data-ttu-id="fc1fe-131">В случае успешного выполнения данный метод возвращает`200 OK` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-131">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc1fe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fc1fe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc1fe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc1fe-133">Request</span></span>
<span data-ttu-id="fc1fe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="fc1fe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc1fe-135">Response</span></span>
<span data-ttu-id="fc1fe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc1fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```




