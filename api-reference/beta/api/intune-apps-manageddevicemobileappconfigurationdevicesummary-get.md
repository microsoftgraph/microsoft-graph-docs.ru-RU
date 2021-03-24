---
title: Получение объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a42f76927ebf587cdbf51afc59cf4546d74ef09e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140142"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="c2075-103">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="c2075-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="c2075-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2075-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2075-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2075-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2075-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2075-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2075-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c2075-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2075-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2075-108">Prerequisites</span></span>
<span data-ttu-id="c2075-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2075-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2075-111">Permission type</span></span>|<span data-ttu-id="c2075-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2075-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2075-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2075-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2075-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2075-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2075-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2075-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2075-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2075-116">Not supported.</span></span>|
|<span data-ttu-id="c2075-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2075-117">Application</span></span>|<span data-ttu-id="c2075-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2075-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2075-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2075-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2075-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2075-120">Optional query parameters</span></span>
<span data-ttu-id="c2075-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2075-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2075-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2075-122">Request headers</span></span>
|<span data-ttu-id="c2075-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2075-123">Header</span></span>|<span data-ttu-id="c2075-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c2075-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2075-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2075-125">Authorization</span></span>|<span data-ttu-id="c2075-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2075-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2075-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c2075-127">Accept</span></span>|<span data-ttu-id="c2075-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2075-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2075-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2075-129">Request body</span></span>
<span data-ttu-id="c2075-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2075-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2075-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2075-131">Response</span></span>
<span data-ttu-id="c2075-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2075-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2075-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2075-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2075-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2075-134">Request</span></span>
<span data-ttu-id="c2075-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2075-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="c2075-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2075-136">Response</span></span>
<span data-ttu-id="c2075-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2075-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```




