---
title: Получение androidForWorkCompliancePolicy
description: Чтение свойства и связи объекта androidForWorkCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6af08fc0c9453e2401036c1538b4be44e8d4f891
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413957"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="ae34d-103">Получение androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ae34d-103">Get androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="ae34d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae34d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae34d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae34d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae34d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae34d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae34d-107">Чтение свойства и связи объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ae34d-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae34d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ae34d-108">Prerequisites</span></span>
<span data-ttu-id="ae34d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae34d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae34d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae34d-111">Permission type</span></span>|<span data-ttu-id="ae34d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae34d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae34d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae34d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae34d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae34d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ae34d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae34d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae34d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae34d-116">Not supported.</span></span>|
|<span data-ttu-id="ae34d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae34d-117">Application</span></span>|<span data-ttu-id="ae34d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae34d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae34d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae34d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae34d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae34d-120">Optional query parameters</span></span>
<span data-ttu-id="ae34d-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae34d-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae34d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae34d-122">Request headers</span></span>
|<span data-ttu-id="ae34d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae34d-123">Header</span></span>|<span data-ttu-id="ae34d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ae34d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae34d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae34d-125">Authorization</span></span>|<span data-ttu-id="ae34d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ae34d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae34d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ae34d-127">Accept</span></span>|<span data-ttu-id="ae34d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ae34d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae34d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae34d-129">Request body</span></span>
<span data-ttu-id="ae34d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae34d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae34d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae34d-131">Response</span></span>
<span data-ttu-id="ae34d-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae34d-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae34d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ae34d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae34d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae34d-134">Request</span></span>
<span data-ttu-id="ae34d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae34d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ae34d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae34d-136">Response</span></span>
<span data-ttu-id="ae34d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae34d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordMinimumLength": 5,
    "passwordRequiredType": "alphabetic",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "securityPreventInstallAppsFromUnknownSources": true,
    "securityDisableUsbDebugging": true,
    "securityRequireVerifyApps": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "securityBlockJailbrokenDevices": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "storageRequireEncryption": true,
    "securityRequireSafetyNetAttestationBasicIntegrity": true,
    "securityRequireSafetyNetAttestationCertifiedDevice": true,
    "securityRequireGooglePlayServices": true,
    "securityRequireUpToDateSecurityProviders": true,
    "securityRequireCompanyPortalAppIntegrity": true
  }
}
```




