---
title: Получение объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57bc506caf7f7c1987a21afbd731b7fab0a36590
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "37358566"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="f146c-103">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f146c-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="f146c-104">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f146c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f146c-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f146c-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f146c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f146c-106">Prerequisites</span></span>
<span data-ttu-id="f146c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f146c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f146c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f146c-109">Permission type</span></span>|<span data-ttu-id="f146c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f146c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f146c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f146c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f146c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f146c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f146c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f146c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f146c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f146c-114">Not supported.</span></span>|
|<span data-ttu-id="f146c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f146c-115">Application</span></span>|<span data-ttu-id="f146c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f146c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f146c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f146c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f146c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f146c-118">Optional query parameters</span></span>
<span data-ttu-id="f146c-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f146c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f146c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f146c-120">Request headers</span></span>
|<span data-ttu-id="f146c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f146c-121">Header</span></span>|<span data-ttu-id="f146c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f146c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f146c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f146c-123">Authorization</span></span>|<span data-ttu-id="f146c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f146c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f146c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f146c-125">Accept</span></span>|<span data-ttu-id="f146c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f146c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f146c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f146c-127">Request body</span></span>
<span data-ttu-id="f146c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f146c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f146c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f146c-129">Response</span></span>
<span data-ttu-id="f146c-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f146c-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f146c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f146c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f146c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f146c-132">Request</span></span>
<span data-ttu-id="f146c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f146c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="f146c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f146c-134">Response</span></span>
<span data-ttu-id="f146c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f146c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




