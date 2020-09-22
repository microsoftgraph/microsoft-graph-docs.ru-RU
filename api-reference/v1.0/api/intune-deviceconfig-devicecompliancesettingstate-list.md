---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61d780cd6c61293aede82ef8dddff32775b4af1b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985267"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="33503-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="33503-103">List deviceComplianceSettingStates</span></span>

<span data-ttu-id="33503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33503-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33503-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33503-106">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="33503-106">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33503-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="33503-107">Prerequisites</span></span>
<span data-ttu-id="33503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33503-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33503-110">Permission type</span></span>|<span data-ttu-id="33503-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33503-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33503-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33503-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33503-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33503-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33503-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33503-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33503-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33503-115">Not supported.</span></span>|
|<span data-ttu-id="33503-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33503-116">Application</span></span>|<span data-ttu-id="33503-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33503-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33503-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33503-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="33503-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33503-119">Request headers</span></span>
|<span data-ttu-id="33503-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33503-120">Header</span></span>|<span data-ttu-id="33503-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33503-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33503-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33503-122">Authorization</span></span>|<span data-ttu-id="33503-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33503-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33503-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33503-124">Accept</span></span>|<span data-ttu-id="33503-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33503-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33503-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33503-126">Request body</span></span>
<span data-ttu-id="33503-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33503-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33503-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="33503-128">Response</span></span>
<span data-ttu-id="33503-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="33503-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33503-130">Пример</span><span class="sxs-lookup"><span data-stu-id="33503-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="33503-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="33503-131">Request</span></span>
<span data-ttu-id="33503-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33503-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="33503-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="33503-133">Response</span></span>
<span data-ttu-id="33503-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33503-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```









