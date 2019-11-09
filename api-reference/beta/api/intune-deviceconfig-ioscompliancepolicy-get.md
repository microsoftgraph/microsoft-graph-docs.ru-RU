---
title: Get iosCompliancePolicy
description: Чтение свойств и связей объекта iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c78c5114c2b13055a31ffecd7f4bbd4adf476e47
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083825"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="1f4e6-103">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1f4e6-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="1f4e6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f4e6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f4e6-106">Чтение свойств и связей объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1f4e6-106">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f4e6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4e6-107">Prerequisites</span></span>
<span data-ttu-id="1f4e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f4e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f4e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4e6-110">Permission type</span></span>|<span data-ttu-id="1f4e6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f4e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f4e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f4e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f4e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f4e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f4e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f4e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f4e6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-115">Not supported.</span></span>|
|<span data-ttu-id="1f4e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f4e6-116">Application</span></span>|<span data-ttu-id="1f4e6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f4e6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f4e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f4e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f4e6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f4e6-119">Optional query parameters</span></span>
<span data-ttu-id="1f4e6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f4e6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f4e6-121">Request headers</span></span>
|<span data-ttu-id="1f4e6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f4e6-122">Header</span></span>|<span data-ttu-id="1f4e6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1f4e6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f4e6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f4e6-124">Authorization</span></span>|<span data-ttu-id="1f4e6-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f4e6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1f4e6-126">Accept</span></span>|<span data-ttu-id="1f4e6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1f4e6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f4e6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f4e6-128">Request body</span></span>
<span data-ttu-id="1f4e6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f4e6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f4e6-130">Response</span></span>
<span data-ttu-id="1f4e6-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-131">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f4e6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1f4e6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f4e6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f4e6-133">Request</span></span>
<span data-ttu-id="1f4e6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="1f4e6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f4e6-135">Response</span></span>
<span data-ttu-id="1f4e6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f4e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






