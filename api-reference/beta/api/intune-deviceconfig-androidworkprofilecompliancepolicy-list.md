---
title: Список androidWorkProfileCompliancePolicies
description: Свойства списка и связей объектов androidWorkProfileCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10796a8fa6fe33e618ece388744cd7f74bdef8c3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398690"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="00df5-103">Список androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="00df5-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="00df5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00df5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00df5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00df5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00df5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00df5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00df5-107">Свойства списка и связей объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="00df5-107">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00df5-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="00df5-108">Prerequisites</span></span>
<span data-ttu-id="00df5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00df5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00df5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00df5-111">Permission type</span></span>|<span data-ttu-id="00df5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00df5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00df5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00df5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00df5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00df5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="00df5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00df5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00df5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00df5-116">Not supported.</span></span>|
|<span data-ttu-id="00df5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00df5-117">Application</span></span>|<span data-ttu-id="00df5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00df5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00df5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00df5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="00df5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00df5-120">Request headers</span></span>
|<span data-ttu-id="00df5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00df5-121">Header</span></span>|<span data-ttu-id="00df5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00df5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00df5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00df5-123">Authorization</span></span>|<span data-ttu-id="00df5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00df5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00df5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00df5-125">Accept</span></span>|<span data-ttu-id="00df5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00df5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00df5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00df5-127">Request body</span></span>
<span data-ttu-id="00df5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00df5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00df5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="00df5-129">Response</span></span>
<span data-ttu-id="00df5-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00df5-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00df5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="00df5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="00df5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="00df5-132">Request</span></span>
<span data-ttu-id="00df5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00df5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="00df5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="00df5-134">Response</span></span>
<span data-ttu-id="00df5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00df5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1620

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "passwordSignInFailureCountBeforeFactoryReset": 12,
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




