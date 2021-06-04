---
title: Получение объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 628594276e0cf271c42881549d1d7275eb0805b8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754226"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="58637-103">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="58637-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="58637-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58637-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58637-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58637-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58637-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="58637-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58637-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58637-107">Prerequisites</span></span>
<span data-ttu-id="58637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58637-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58637-110">Permission type</span></span>|<span data-ttu-id="58637-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58637-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58637-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58637-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58637-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58637-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58637-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58637-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58637-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58637-115">Not supported.</span></span>|
|<span data-ttu-id="58637-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="58637-116">Application</span></span>|<span data-ttu-id="58637-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58637-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58637-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58637-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58637-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58637-119">Optional query parameters</span></span>
<span data-ttu-id="58637-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58637-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58637-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58637-121">Request headers</span></span>
|<span data-ttu-id="58637-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58637-122">Header</span></span>|<span data-ttu-id="58637-123">Значение</span><span class="sxs-lookup"><span data-stu-id="58637-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58637-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="58637-124">Authorization</span></span>|<span data-ttu-id="58637-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58637-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58637-126">Accept</span><span class="sxs-lookup"><span data-stu-id="58637-126">Accept</span></span>|<span data-ttu-id="58637-127">application/json</span><span class="sxs-lookup"><span data-stu-id="58637-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58637-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58637-128">Request body</span></span>
<span data-ttu-id="58637-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58637-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58637-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="58637-130">Response</span></span>
<span data-ttu-id="58637-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58637-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58637-132">Пример</span><span class="sxs-lookup"><span data-stu-id="58637-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="58637-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="58637-133">Request</span></span>
<span data-ttu-id="58637-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58637-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="58637-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="58637-135">Response</span></span>
<span data-ttu-id="58637-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58637-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```




