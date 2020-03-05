---
title: Get windows10MobileCompliancePolicy
description: Чтение свойств и связей объекта windows10MobileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ac276c7c04d6ab403a8093c1bdcb59a7be93e5c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42479067"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="2b978-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2b978-103">Get windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="2b978-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b978-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b978-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b978-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b978-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b978-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b978-107">Чтение свойств и связей объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b978-107">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b978-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2b978-108">Prerequisites</span></span>
<span data-ttu-id="2b978-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b978-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b978-111">Permission type</span></span>|<span data-ttu-id="2b978-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b978-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b978-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b978-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b978-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b978-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2b978-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b978-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b978-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b978-116">Not supported.</span></span>|
|<span data-ttu-id="2b978-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b978-117">Application</span></span>|<span data-ttu-id="2b978-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b978-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b978-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b978-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b978-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b978-120">Optional query parameters</span></span>
<span data-ttu-id="2b978-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b978-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b978-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b978-122">Request headers</span></span>
|<span data-ttu-id="2b978-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b978-123">Header</span></span>|<span data-ttu-id="2b978-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2b978-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b978-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b978-125">Authorization</span></span>|<span data-ttu-id="2b978-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b978-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b978-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2b978-127">Accept</span></span>|<span data-ttu-id="2b978-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2b978-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b978-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b978-129">Request body</span></span>
<span data-ttu-id="2b978-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b978-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b978-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b978-131">Response</span></span>
<span data-ttu-id="2b978-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b978-132">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b978-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2b978-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b978-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b978-134">Request</span></span>
<span data-ttu-id="2b978-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b978-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="2b978-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b978-136">Response</span></span>
<span data-ttu-id="2b978-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b978-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "value": {
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
}
```





