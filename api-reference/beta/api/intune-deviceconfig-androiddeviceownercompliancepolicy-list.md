---
title: Список АндроиддевицеовнеркомплианцеполиЦиес
description: Список свойств и связей объектов Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c6879838bbfba19e5ba424061c7332c398547af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444205"
---
# <a name="list-androiddeviceownercompliancepolicies"></a><span data-ttu-id="3ea35-103">Список АндроиддевицеовнеркомплианцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="3ea35-103">List androidDeviceOwnerCompliancePolicies</span></span>

<span data-ttu-id="3ea35-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3ea35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ea35-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ea35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ea35-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ea35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ea35-107">Список свойств и связей объектов [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3ea35-107">List properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ea35-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ea35-108">Prerequisites</span></span>
<span data-ttu-id="3ea35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ea35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea35-111">Permission type</span></span>|<span data-ttu-id="3ea35-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ea35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ea35-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea35-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ea35-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ea35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ea35-116">Not supported.</span></span>|
|<span data-ttu-id="3ea35-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ea35-117">Application</span></span>|<span data-ttu-id="3ea35-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea35-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ea35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3ea35-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ea35-120">Request headers</span></span>
|<span data-ttu-id="3ea35-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ea35-121">Header</span></span>|<span data-ttu-id="3ea35-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ea35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ea35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ea35-123">Authorization</span></span>|<span data-ttu-id="3ea35-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ea35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ea35-125">Accept</span></span>|<span data-ttu-id="3ea35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ea35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ea35-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ea35-127">Request body</span></span>
<span data-ttu-id="3ea35-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ea35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ea35-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ea35-129">Response</span></span>
<span data-ttu-id="3ea35-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ea35-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ea35-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3ea35-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ea35-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea35-132">Request</span></span>
<span data-ttu-id="3ea35-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ea35-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="3ea35-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea35-134">Response</span></span>
<span data-ttu-id="3ea35-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ea35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1552

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "be2464b4-64b4-be24-b464-24beb46424be",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "advancedThreatProtectionRequiredSecurityLevel": "secured",
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordMinimumLetterCharacters": 15,
      "passwordMinimumLowerCaseCharacters": 2,
      "passwordMinimumNonLetterCharacters": 2,
      "passwordMinimumNumericCharacters": 0,
      "passwordMinimumSymbolCharacters": 15,
      "passwordMinimumUpperCaseCharacters": 2,
      "passwordRequiredType": "required",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordCountToBlock": 4,
      "storageRequireEncryption": true
    }
  ]
}
```





