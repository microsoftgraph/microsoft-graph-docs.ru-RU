---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b05be3f4176eeac3214bfc81310272c689c1e0a6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387609"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="43c98-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="43c98-103">List settingStateDeviceSummaries</span></span>

<span data-ttu-id="43c98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43c98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43c98-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43c98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c98-106">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="43c98-106">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43c98-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="43c98-107">Prerequisites</span></span>
<span data-ttu-id="43c98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43c98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c98-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43c98-110">Permission type</span></span>|<span data-ttu-id="43c98-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43c98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43c98-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43c98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43c98-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43c98-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43c98-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43c98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43c98-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43c98-115">Not supported.</span></span>|
|<span data-ttu-id="43c98-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43c98-116">Application</span></span>|<span data-ttu-id="43c98-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43c98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43c98-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43c98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="43c98-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43c98-119">Request headers</span></span>
|<span data-ttu-id="43c98-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43c98-120">Header</span></span>|<span data-ttu-id="43c98-121">Значение</span><span class="sxs-lookup"><span data-stu-id="43c98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43c98-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43c98-122">Authorization</span></span>|<span data-ttu-id="43c98-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43c98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43c98-124">Accept</span><span class="sxs-lookup"><span data-stu-id="43c98-124">Accept</span></span>|<span data-ttu-id="43c98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43c98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c98-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43c98-126">Request body</span></span>
<span data-ttu-id="43c98-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43c98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c98-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="43c98-128">Response</span></span>
<span data-ttu-id="43c98-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43c98-129">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43c98-130">Пример</span><span class="sxs-lookup"><span data-stu-id="43c98-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c98-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="43c98-131">Request</span></span>
<span data-ttu-id="43c98-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43c98-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="43c98-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c98-133">Response</span></span>
<span data-ttu-id="43c98-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43c98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```






