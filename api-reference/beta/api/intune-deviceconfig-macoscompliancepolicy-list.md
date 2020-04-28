---
title: Перечисление объектов macOSCompliancePolicy
description: Список свойств и связей объектов macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c080bdcb04b2468e656dfce3c97a1f46f560e34d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438319"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="30e70-103">Перечисление объектов macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="30e70-103">List macOSCompliancePolicies</span></span>

<span data-ttu-id="30e70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30e70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30e70-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30e70-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30e70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30e70-107">Список свойств и связей объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30e70-107">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30e70-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30e70-108">Prerequisites</span></span>
<span data-ttu-id="30e70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30e70-111">Permission type</span></span>|<span data-ttu-id="30e70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30e70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30e70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30e70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30e70-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e70-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30e70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30e70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30e70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e70-116">Not supported.</span></span>|
|<span data-ttu-id="30e70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30e70-117">Application</span></span>|<span data-ttu-id="30e70-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e70-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30e70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30e70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="30e70-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30e70-120">Request headers</span></span>
|<span data-ttu-id="30e70-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30e70-121">Header</span></span>|<span data-ttu-id="30e70-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30e70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30e70-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30e70-123">Authorization</span></span>|<span data-ttu-id="30e70-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30e70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30e70-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30e70-125">Accept</span></span>|<span data-ttu-id="30e70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30e70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30e70-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30e70-127">Request body</span></span>
<span data-ttu-id="30e70-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30e70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30e70-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="30e70-129">Response</span></span>
<span data-ttu-id="30e70-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30e70-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e70-131">Пример</span><span class="sxs-lookup"><span data-stu-id="30e70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="30e70-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="30e70-132">Request</span></span>
<span data-ttu-id="30e70-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30e70-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="30e70-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="30e70-134">Response</span></span>
<span data-ttu-id="30e70-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30e70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "osMinimumBuildVersion": "Os Minimum Build Version value",
      "osMaximumBuildVersion": "Os Maximum Build Version value",
      "systemIntegrityProtectionEnabled": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "storageRequireEncryption": true,
      "gatekeeperAllowedAppSource": "macAppStore",
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true
    }
  ]
}
```



