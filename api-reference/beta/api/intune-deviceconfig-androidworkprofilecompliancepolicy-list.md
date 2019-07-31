---
title: Список АндроидворкпрофилекомплианцеполиЦиес
description: Список свойств и связей объектов androidWorkProfileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea90baf1a57d42000ccf54fd5b28f8192ecc157d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951024"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="395f8-103">Список АндроидворкпрофилекомплианцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="395f8-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="395f8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="395f8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="395f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="395f8-106">Список свойств и связей объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="395f8-106">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="395f8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="395f8-107">Prerequisites</span></span>
<span data-ttu-id="395f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="395f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="395f8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="395f8-110">Permission type</span></span>|<span data-ttu-id="395f8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="395f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="395f8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="395f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="395f8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="395f8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="395f8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="395f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="395f8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395f8-115">Not supported.</span></span>|
|<span data-ttu-id="395f8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="395f8-116">Application</span></span>|<span data-ttu-id="395f8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395f8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="395f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="395f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="395f8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="395f8-119">Request headers</span></span>
|<span data-ttu-id="395f8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="395f8-120">Header</span></span>|<span data-ttu-id="395f8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="395f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="395f8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="395f8-122">Authorization</span></span>|<span data-ttu-id="395f8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="395f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="395f8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="395f8-124">Accept</span></span>|<span data-ttu-id="395f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="395f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="395f8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="395f8-126">Request body</span></span>
<span data-ttu-id="395f8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="395f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="395f8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="395f8-128">Response</span></span>
<span data-ttu-id="395f8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="395f8-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="395f8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="395f8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="395f8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="395f8-131">Request</span></span>
<span data-ttu-id="395f8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="395f8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="395f8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="395f8-133">Response</span></span>
<span data-ttu-id="395f8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="395f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





