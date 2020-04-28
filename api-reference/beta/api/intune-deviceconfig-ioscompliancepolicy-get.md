---
title: Get iosCompliancePolicy
description: Чтение свойств и связей объекта iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 398265886076befa31260184f6b235040fa31c22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432982"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="fece3-103">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fece3-103">Get iosCompliancePolicy</span></span>

<span data-ttu-id="fece3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fece3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fece3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fece3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fece3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fece3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fece3-107">Чтение свойств и связей объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fece3-107">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fece3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fece3-108">Prerequisites</span></span>
<span data-ttu-id="fece3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fece3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fece3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fece3-111">Permission type</span></span>|<span data-ttu-id="fece3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fece3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fece3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fece3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fece3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fece3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fece3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fece3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fece3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fece3-116">Not supported.</span></span>|
|<span data-ttu-id="fece3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fece3-117">Application</span></span>|<span data-ttu-id="fece3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fece3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fece3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fece3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fece3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fece3-120">Optional query parameters</span></span>
<span data-ttu-id="fece3-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fece3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fece3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fece3-122">Request headers</span></span>
|<span data-ttu-id="fece3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fece3-123">Header</span></span>|<span data-ttu-id="fece3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fece3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fece3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fece3-125">Authorization</span></span>|<span data-ttu-id="fece3-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fece3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fece3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fece3-127">Accept</span></span>|<span data-ttu-id="fece3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fece3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fece3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fece3-129">Request body</span></span>
<span data-ttu-id="fece3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fece3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fece3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fece3-131">Response</span></span>
<span data-ttu-id="fece3-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fece3-132">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fece3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fece3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fece3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fece3-134">Request</span></span>
<span data-ttu-id="fece3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fece3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fece3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fece3-136">Response</span></span>
<span data-ttu-id="fece3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fece3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1504

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



