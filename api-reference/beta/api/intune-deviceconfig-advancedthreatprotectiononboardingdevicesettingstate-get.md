---
title: Получение Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Чтение свойств и связей объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1923b77c9be1cd86b84110bcac0f2bfda703d97a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954078"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="4999d-103">Получение Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="4999d-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="4999d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4999d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4999d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4999d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4999d-106">Чтение свойств и связей объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="4999d-106">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4999d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4999d-107">Prerequisites</span></span>
<span data-ttu-id="4999d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4999d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4999d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4999d-110">Permission type</span></span>|<span data-ttu-id="4999d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4999d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4999d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4999d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4999d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4999d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4999d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4999d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4999d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4999d-115">Not supported.</span></span>|
|<span data-ttu-id="4999d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4999d-116">Application</span></span>|<span data-ttu-id="4999d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4999d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4999d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4999d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4999d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4999d-119">Optional query parameters</span></span>
<span data-ttu-id="4999d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4999d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4999d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4999d-121">Request headers</span></span>
|<span data-ttu-id="4999d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4999d-122">Header</span></span>|<span data-ttu-id="4999d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4999d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4999d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4999d-124">Authorization</span></span>|<span data-ttu-id="4999d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4999d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4999d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4999d-126">Accept</span></span>|<span data-ttu-id="4999d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4999d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4999d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4999d-128">Request body</span></span>
<span data-ttu-id="4999d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4999d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4999d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4999d-130">Response</span></span>
<span data-ttu-id="4999d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4999d-131">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4999d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4999d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4999d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4999d-133">Request</span></span>
<span data-ttu-id="4999d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4999d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="4999d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4999d-135">Response</span></span>
<span data-ttu-id="4999d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4999d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





