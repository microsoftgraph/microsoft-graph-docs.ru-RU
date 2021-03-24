---
title: Get iosCompliancePolicy
description: Чтение свойств и связей объекта iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca43235e755e12a23a842236f936535c2bb40bd4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127993"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="46da5-103">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="46da5-103">Get iosCompliancePolicy</span></span>

<span data-ttu-id="46da5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46da5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46da5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46da5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46da5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46da5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46da5-107">Чтение свойств и связей объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="46da5-107">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46da5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="46da5-108">Prerequisites</span></span>
<span data-ttu-id="46da5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46da5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46da5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46da5-111">Permission type</span></span>|<span data-ttu-id="46da5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46da5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46da5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46da5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46da5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46da5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46da5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46da5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46da5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46da5-116">Not supported.</span></span>|
|<span data-ttu-id="46da5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="46da5-117">Application</span></span>|<span data-ttu-id="46da5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46da5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46da5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46da5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46da5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46da5-120">Optional query parameters</span></span>
<span data-ttu-id="46da5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="46da5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46da5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46da5-122">Request headers</span></span>
|<span data-ttu-id="46da5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46da5-123">Header</span></span>|<span data-ttu-id="46da5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="46da5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46da5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="46da5-125">Authorization</span></span>|<span data-ttu-id="46da5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46da5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46da5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="46da5-127">Accept</span></span>|<span data-ttu-id="46da5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="46da5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46da5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46da5-129">Request body</span></span>
<span data-ttu-id="46da5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46da5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46da5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="46da5-131">Response</span></span>
<span data-ttu-id="46da5-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="46da5-132">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46da5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="46da5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="46da5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="46da5-134">Request</span></span>
<span data-ttu-id="46da5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46da5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="46da5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="46da5-136">Response</span></span>
<span data-ttu-id="46da5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46da5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1569

{
  "value": {
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
    "advancedThreatProtectionRequiredSecurityLevel": "secured",
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
}
```




