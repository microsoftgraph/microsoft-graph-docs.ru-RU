---
title: Список Адванцедсреатпротектиононбоардингдевицесеттингстатес
description: Список свойств и связей объектов Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba28fe2f29882ff17192cc0ef7370b7aee761078
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933433"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="ab01b-103">Список Адванцедсреатпротектиононбоардингдевицесеттингстатес</span><span class="sxs-lookup"><span data-stu-id="ab01b-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

> <span data-ttu-id="ab01b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab01b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab01b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab01b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab01b-106">Список свойств и связей объектов [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ab01b-106">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab01b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab01b-107">Prerequisites</span></span>
<span data-ttu-id="ab01b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab01b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab01b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab01b-110">Permission type</span></span>|<span data-ttu-id="ab01b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab01b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab01b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab01b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab01b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab01b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab01b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab01b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab01b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab01b-115">Not supported.</span></span>|
|<span data-ttu-id="ab01b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab01b-116">Application</span></span>|<span data-ttu-id="ab01b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab01b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab01b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab01b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="ab01b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab01b-119">Request headers</span></span>
|<span data-ttu-id="ab01b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab01b-120">Header</span></span>|<span data-ttu-id="ab01b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab01b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab01b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab01b-122">Authorization</span></span>|<span data-ttu-id="ab01b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab01b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab01b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ab01b-124">Accept</span></span>|<span data-ttu-id="ab01b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab01b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab01b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab01b-126">Request body</span></span>
<span data-ttu-id="ab01b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab01b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab01b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab01b-128">Response</span></span>
<span data-ttu-id="ab01b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab01b-129">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab01b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ab01b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab01b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab01b-131">Request</span></span>
<span data-ttu-id="ab01b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab01b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="ab01b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab01b-133">Response</span></span>
<span data-ttu-id="ab01b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab01b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




