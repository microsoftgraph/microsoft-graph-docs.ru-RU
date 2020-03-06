---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43f95ceef6ba6fd348e48c0be6562373b8e74da8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514924"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="4b878-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="4b878-103">List deviceComplianceSettingStates</span></span>

<span data-ttu-id="4b878-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b878-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b878-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b878-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b878-106">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="4b878-106">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b878-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4b878-107">Prerequisites</span></span>
<span data-ttu-id="4b878-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b878-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b878-110">Permission type</span></span>|<span data-ttu-id="4b878-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b878-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b878-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b878-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b878-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b878-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b878-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b878-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b878-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b878-115">Not supported.</span></span>|
|<span data-ttu-id="4b878-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b878-116">Application</span></span>|<span data-ttu-id="4b878-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b878-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b878-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b878-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="4b878-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b878-119">Request headers</span></span>
|<span data-ttu-id="4b878-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b878-120">Header</span></span>|<span data-ttu-id="4b878-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b878-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b878-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b878-122">Authorization</span></span>|<span data-ttu-id="4b878-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b878-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b878-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b878-124">Accept</span></span>|<span data-ttu-id="4b878-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b878-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b878-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b878-126">Request body</span></span>
<span data-ttu-id="4b878-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b878-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b878-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b878-128">Response</span></span>
<span data-ttu-id="4b878-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b878-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b878-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4b878-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b878-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b878-131">Request</span></span>
<span data-ttu-id="4b878-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b878-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="4b878-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b878-133">Response</span></span>
<span data-ttu-id="4b878-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b878-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




