---
title: Перечисление объектов iosCompliancePolicy
description: Список свойств и связей объектов iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8215e22e99fe181ade1a302f8c8a75ec81587871
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082730"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="a90a3-103">Перечисление объектов iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a90a3-103">List iosCompliancePolicies</span></span>

<span data-ttu-id="a90a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a90a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a90a3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a90a3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a90a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a90a3-107">Список свойств и связей объектов [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a90a3-107">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a90a3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a90a3-108">Prerequisites</span></span>
<span data-ttu-id="a90a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a90a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a90a3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a90a3-111">Permission type</span></span>|<span data-ttu-id="a90a3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a90a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a90a3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a90a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a90a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a90a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a90a3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a90a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a90a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a3-116">Not supported.</span></span>|
|<span data-ttu-id="a90a3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a90a3-117">Application</span></span>|<span data-ttu-id="a90a3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a90a3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a90a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a90a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a90a3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a90a3-120">Request headers</span></span>
|<span data-ttu-id="a90a3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a90a3-121">Header</span></span>|<span data-ttu-id="a90a3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a90a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a90a3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a90a3-123">Authorization</span></span>|<span data-ttu-id="a90a3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a90a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a90a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a90a3-125">Accept</span></span>|<span data-ttu-id="a90a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a90a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a90a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a90a3-127">Request body</span></span>
<span data-ttu-id="a90a3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a90a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a90a3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a90a3-129">Response</span></span>
<span data-ttu-id="a90a3-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a90a3-130">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a90a3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a90a3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a90a3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a90a3-132">Request</span></span>
<span data-ttu-id="a90a3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a90a3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="a90a3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a90a3-134">Response</span></span>
<span data-ttu-id="a90a3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a90a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1590

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4f501351-1351-4f50-5113-504f5113504f",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "osMinimumBuildVersion": "Os Minimum Build Version value",
      "osMaximumBuildVersion": "Os Maximum Build Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true,
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```






