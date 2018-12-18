---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 8d231c2578ebeb3a88372dbc765806a67bdeff3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313708"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="15d0c-103">Перечисление объектов androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="15d0c-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="15d0c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15d0c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15d0c-105">Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="15d0c-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15d0c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15d0c-106">Prerequisites</span></span>
<span data-ttu-id="15d0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15d0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15d0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15d0c-109">Permission type</span></span>|<span data-ttu-id="15d0c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15d0c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15d0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15d0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15d0c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15d0c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="15d0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15d0c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15d0c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15d0c-114">Not supported.</span></span>|
|<span data-ttu-id="15d0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15d0c-115">Application</span></span>|<span data-ttu-id="15d0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15d0c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15d0c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15d0c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="15d0c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15d0c-118">Request headers</span></span>
|<span data-ttu-id="15d0c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15d0c-119">Header</span></span>|<span data-ttu-id="15d0c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="15d0c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15d0c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15d0c-121">Authorization</span></span>|<span data-ttu-id="15d0c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="15d0c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15d0c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="15d0c-123">Accept</span></span>|<span data-ttu-id="15d0c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="15d0c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15d0c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15d0c-125">Request body</span></span>
<span data-ttu-id="15d0c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15d0c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15d0c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="15d0c-127">Response</span></span>
<span data-ttu-id="15d0c-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15d0c-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15d0c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="15d0c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="15d0c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="15d0c-130">Request</span></span>
<span data-ttu-id="15d0c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15d0c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="15d0c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="15d0c-132">Response</span></span>
<span data-ttu-id="15d0c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15d0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
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



