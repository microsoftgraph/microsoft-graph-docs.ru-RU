---
title: Получение Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Чтение свойств и связей объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cc2c9b4e8e25ac34bfca3851c2fecab6b852b58
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49243437"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="2e51e-103">Получение Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="2e51e-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="2e51e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e51e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e51e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e51e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e51e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e51e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e51e-107">Чтение свойств и связей объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="2e51e-107">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e51e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e51e-108">Prerequisites</span></span>
<span data-ttu-id="2e51e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e51e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e51e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e51e-111">Permission type</span></span>|<span data-ttu-id="2e51e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e51e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e51e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e51e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e51e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e51e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e51e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e51e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e51e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e51e-116">Not supported.</span></span>|
|<span data-ttu-id="2e51e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e51e-117">Application</span></span>|<span data-ttu-id="2e51e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e51e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e51e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e51e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e51e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e51e-120">Optional query parameters</span></span>
<span data-ttu-id="2e51e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e51e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e51e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e51e-122">Request headers</span></span>
|<span data-ttu-id="2e51e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e51e-123">Header</span></span>|<span data-ttu-id="2e51e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2e51e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e51e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e51e-125">Authorization</span></span>|<span data-ttu-id="2e51e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e51e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e51e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2e51e-127">Accept</span></span>|<span data-ttu-id="2e51e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2e51e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e51e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e51e-129">Request body</span></span>
<span data-ttu-id="2e51e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e51e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e51e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e51e-131">Response</span></span>
<span data-ttu-id="2e51e-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e51e-132">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e51e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2e51e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e51e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e51e-134">Request</span></span>
<span data-ttu-id="2e51e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e51e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="2e51e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e51e-136">Response</span></span>
<span data-ttu-id="2e51e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e51e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




