---
title: Перечисление объектов windows10MobileCompliancePolicy
description: Список свойств и связей объектов windows10MobileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ea2cf01ef42df5b70de06535cdbc693ccc9c9f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42479053"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="1ebe6-103">Перечисление объектов windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1ebe6-103">List windows10MobileCompliancePolicies</span></span>

<span data-ttu-id="1ebe6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1ebe6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ebe6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ebe6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ebe6-107">Список свойств и связей объектов [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1ebe6-107">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ebe6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1ebe6-108">Prerequisites</span></span>
<span data-ttu-id="1ebe6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ebe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ebe6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ebe6-111">Permission type</span></span>|<span data-ttu-id="1ebe6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ebe6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ebe6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ebe6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ebe6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ebe6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ebe6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ebe6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ebe6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-116">Not supported.</span></span>|
|<span data-ttu-id="1ebe6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ebe6-117">Application</span></span>|<span data-ttu-id="1ebe6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ebe6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ebe6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ebe6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1ebe6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1ebe6-120">Request headers</span></span>
|<span data-ttu-id="1ebe6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ebe6-121">Header</span></span>|<span data-ttu-id="1ebe6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ebe6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ebe6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ebe6-123">Authorization</span></span>|<span data-ttu-id="1ebe6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ebe6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ebe6-125">Accept</span></span>|<span data-ttu-id="1ebe6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ebe6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ebe6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ebe6-127">Request body</span></span>
<span data-ttu-id="1ebe6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ebe6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ebe6-129">Response</span></span>
<span data-ttu-id="1ebe6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-130">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ebe6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1ebe6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ebe6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ebe6-132">Request</span></span>
<span data-ttu-id="1ebe6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="1ebe6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ebe6-134">Response</span></span>
<span data-ttu-id="1ebe6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ebe6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3d4237b0-37b0-3d42-b037-423db037423d",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordExpirationDays": 6,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordRequireToUnlockFromIdle": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ]
    }
  ]
}
```





