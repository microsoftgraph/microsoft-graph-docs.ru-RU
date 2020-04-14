---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15f89d5e88047a99eaf06c555bb350005f781574
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433803"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="98d48-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="98d48-103">List deviceComplianceSettingStates</span></span>

<span data-ttu-id="98d48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98d48-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98d48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98d48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98d48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98d48-107">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="98d48-107">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98d48-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="98d48-108">Prerequisites</span></span>
<span data-ttu-id="98d48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98d48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98d48-111">Permission type</span></span>|<span data-ttu-id="98d48-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98d48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98d48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98d48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98d48-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d48-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="98d48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98d48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98d48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98d48-116">Not supported.</span></span>|
|<span data-ttu-id="98d48-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="98d48-117">Application</span></span>|<span data-ttu-id="98d48-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d48-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98d48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98d48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="98d48-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98d48-120">Request headers</span></span>
|<span data-ttu-id="98d48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98d48-121">Header</span></span>|<span data-ttu-id="98d48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98d48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98d48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d48-123">Authorization</span></span>|<span data-ttu-id="98d48-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98d48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98d48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98d48-125">Accept</span></span>|<span data-ttu-id="98d48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98d48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98d48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98d48-127">Request body</span></span>
<span data-ttu-id="98d48-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98d48-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d48-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="98d48-129">Response</span></span>
<span data-ttu-id="98d48-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98d48-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98d48-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98d48-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="98d48-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98d48-132">Request</span></span>
<span data-ttu-id="98d48-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98d48-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="98d48-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98d48-134">Response</span></span>
<span data-ttu-id="98d48-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98d48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "platformType": "windowsRT",
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



