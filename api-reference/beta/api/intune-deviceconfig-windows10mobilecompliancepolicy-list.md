---
title: Перечисление объектов windows10MobileCompliancePolicy
description: Список свойств и связей объектов windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 937a3603c4a17c2cd845417625609f6b6f2ea6b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516541"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="d90e7-103">Перечисление объектов windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d90e7-103">List windows10MobileCompliancePolicies</span></span>

> <span data-ttu-id="d90e7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d90e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d90e7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d90e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90e7-106">Список свойств и связей объектов [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d90e7-106">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d90e7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d90e7-107">Prerequisites</span></span>
<span data-ttu-id="d90e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d90e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d90e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d90e7-110">Permission type</span></span>|<span data-ttu-id="d90e7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d90e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d90e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d90e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d90e7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d90e7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d90e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d90e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d90e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d90e7-115">Not supported.</span></span>|
|<span data-ttu-id="d90e7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d90e7-116">Application</span></span>|<span data-ttu-id="d90e7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d90e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d90e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d90e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d90e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d90e7-119">Request headers</span></span>
|<span data-ttu-id="d90e7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d90e7-120">Header</span></span>|<span data-ttu-id="d90e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d90e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d90e7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d90e7-122">Authorization</span></span>|<span data-ttu-id="d90e7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d90e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d90e7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d90e7-124">Accept</span></span>|<span data-ttu-id="d90e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d90e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d90e7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d90e7-126">Request body</span></span>
<span data-ttu-id="d90e7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d90e7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d90e7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d90e7-128">Response</span></span>
<span data-ttu-id="d90e7-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d90e7-129">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d90e7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d90e7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d90e7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d90e7-131">Request</span></span>
<span data-ttu-id="d90e7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d90e7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d90e7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d90e7-133">Response</span></span>
<span data-ttu-id="d90e7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d90e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





