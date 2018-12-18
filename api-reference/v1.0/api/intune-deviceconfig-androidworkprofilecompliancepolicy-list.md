---
title: Список androidWorkProfileCompliancePolicies
description: Свойства списка и связей объектов androidWorkProfileCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: d8d63acf4f9c0d3966ab4eb488b2e08747dc7c01
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331586"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="82f02-103">Список androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="82f02-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="82f02-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82f02-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82f02-105">Свойства списка и связей объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="82f02-105">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82f02-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82f02-106">Prerequisites</span></span>
<span data-ttu-id="82f02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f02-109">Permission type</span></span>|<span data-ttu-id="82f02-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f02-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82f02-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82f02-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82f02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f02-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f02-114">Not supported.</span></span>|
|<span data-ttu-id="82f02-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f02-115">Application</span></span>|<span data-ttu-id="82f02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f02-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f02-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="82f02-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82f02-118">Request headers</span></span>
|<span data-ttu-id="82f02-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82f02-119">Header</span></span>|<span data-ttu-id="82f02-120">Значение</span><span class="sxs-lookup"><span data-stu-id="82f02-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82f02-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82f02-121">Authorization</span></span>|<span data-ttu-id="82f02-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82f02-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82f02-123">Accept</span><span class="sxs-lookup"><span data-stu-id="82f02-123">Accept</span></span>|<span data-ttu-id="82f02-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82f02-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82f02-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82f02-125">Request body</span></span>
<span data-ttu-id="82f02-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82f02-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82f02-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="82f02-127">Response</span></span>
<span data-ttu-id="82f02-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="82f02-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82f02-129">Пример</span><span class="sxs-lookup"><span data-stu-id="82f02-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="82f02-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f02-130">Request</span></span>
<span data-ttu-id="82f02-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f02-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="82f02-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="82f02-132">Response</span></span>
<span data-ttu-id="82f02-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="82f02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "id": "4e385271-5271-4e38-7152-384e7152384e",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```



