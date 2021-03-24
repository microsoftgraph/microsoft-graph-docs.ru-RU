---
title: Список advancedThreatProtectionOnboardingDeviceSettingStates
description: Список свойств и связей объектов advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f19e5b5b99ee9555d4f5dbc84fe9ede16e87191
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126894"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="0c545-103">Список advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="0c545-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

<span data-ttu-id="0c545-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c545-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c545-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c545-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c545-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c545-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c545-107">Список свойств и связей объектов [advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="0c545-107">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c545-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c545-108">Prerequisites</span></span>
<span data-ttu-id="0c545-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c545-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c545-111">Permission type</span></span>|<span data-ttu-id="0c545-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c545-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c545-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c545-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c545-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c545-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c545-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c545-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c545-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c545-116">Not supported.</span></span>|
|<span data-ttu-id="0c545-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c545-117">Application</span></span>|<span data-ttu-id="0c545-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c545-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c545-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c545-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="0c545-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c545-120">Request headers</span></span>
|<span data-ttu-id="0c545-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c545-121">Header</span></span>|<span data-ttu-id="0c545-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c545-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c545-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c545-123">Authorization</span></span>|<span data-ttu-id="0c545-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c545-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c545-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c545-125">Accept</span></span>|<span data-ttu-id="0c545-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c545-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c545-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c545-127">Request body</span></span>
<span data-ttu-id="0c545-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c545-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c545-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c545-129">Response</span></span>
<span data-ttu-id="0c545-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0c545-130">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c545-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0c545-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c545-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c545-132">Request</span></span>
<span data-ttu-id="0c545-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c545-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="0c545-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c545-134">Response</span></span>
<span data-ttu-id="0c545-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c545-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
      "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
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




