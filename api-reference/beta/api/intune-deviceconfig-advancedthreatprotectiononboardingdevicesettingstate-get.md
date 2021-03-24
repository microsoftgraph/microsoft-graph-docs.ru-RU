---
title: Get advancedThreatProtectionOnboardingDeviceSettingState
description: Чтение свойств и связей объекта advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c0db77b75afb6b9408d27e384d87f155db4bb6d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126901"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="cc3c0-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="cc3c0-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="cc3c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc3c0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc3c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc3c0-107">Чтение свойств и связей объекта [advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="cc3c0-107">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc3c0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc3c0-108">Prerequisites</span></span>
<span data-ttu-id="cc3c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc3c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc3c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc3c0-111">Permission type</span></span>|<span data-ttu-id="cc3c0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc3c0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc3c0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc3c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc3c0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc3c0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc3c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc3c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-116">Not supported.</span></span>|
|<span data-ttu-id="cc3c0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc3c0-117">Application</span></span>|<span data-ttu-id="cc3c0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc3c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc3c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc3c0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc3c0-120">Optional query parameters</span></span>
<span data-ttu-id="cc3c0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc3c0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc3c0-122">Request headers</span></span>
|<span data-ttu-id="cc3c0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc3c0-123">Header</span></span>|<span data-ttu-id="cc3c0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cc3c0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc3c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc3c0-125">Authorization</span></span>|<span data-ttu-id="cc3c0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc3c0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cc3c0-127">Accept</span></span>|<span data-ttu-id="cc3c0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cc3c0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc3c0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc3c0-129">Request body</span></span>
<span data-ttu-id="cc3c0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc3c0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc3c0-131">Response</span></span>
<span data-ttu-id="cc3c0-132">В случае успешной работы этот метод возвращает код ответа и расширенный `200 OK` [объектThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-132">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3c0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cc3c0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc3c0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc3c0-134">Request</span></span>
<span data-ttu-id="cc3c0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="cc3c0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc3c0-136">Response</span></span>
<span data-ttu-id="cc3c0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc3c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
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
}
```




