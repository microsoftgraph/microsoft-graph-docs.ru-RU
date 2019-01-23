---
title: Get windows10CompliancePolicy
description: Чтение свойств и связей объекта windows10CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a511004d170aa53be2d15bcad5387592288c49df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414433"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="93b0c-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="93b0c-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="93b0c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93b0c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="93b0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93b0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93b0c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93b0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93b0c-107">Чтение свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93b0c-107">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93b0c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="93b0c-108">Prerequisites</span></span>
<span data-ttu-id="93b0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93b0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93b0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93b0c-111">Permission type</span></span>|<span data-ttu-id="93b0c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93b0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93b0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93b0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93b0c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93b0c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="93b0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93b0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93b0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93b0c-116">Not supported.</span></span>|
|<span data-ttu-id="93b0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93b0c-117">Application</span></span>|<span data-ttu-id="93b0c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93b0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93b0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93b0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93b0c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93b0c-120">Optional query parameters</span></span>
<span data-ttu-id="93b0c-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="93b0c-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93b0c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93b0c-122">Request headers</span></span>
|<span data-ttu-id="93b0c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93b0c-123">Header</span></span>|<span data-ttu-id="93b0c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="93b0c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93b0c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="93b0c-125">Authorization</span></span>|<span data-ttu-id="93b0c-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="93b0c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93b0c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="93b0c-127">Accept</span></span>|<span data-ttu-id="93b0c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="93b0c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93b0c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93b0c-129">Request body</span></span>
<span data-ttu-id="93b0c-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93b0c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93b0c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="93b0c-131">Response</span></span>
<span data-ttu-id="93b0c-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93b0c-132">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93b0c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="93b0c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="93b0c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="93b0c-134">Request</span></span>
<span data-ttu-id="93b0c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93b0c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="93b0c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b0c-136">Response</span></span>
<span data-ttu-id="93b0c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="93b0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1951

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2919ae62-ae62-2919-62ae-192962ae1929",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordRequiredToUnlockFromIdle": true,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "requireHealthyDeviceReport": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
    "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "defenderEnabled": true,
    "defenderVersion": "Defender Version value",
    "signatureOutOfDate": true,
    "rtpEnabled": true,
    "antivirusRequired": true,
    "antiSpywareRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ],
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "configurationManagerComplianceRequired": true
  }
}
```




