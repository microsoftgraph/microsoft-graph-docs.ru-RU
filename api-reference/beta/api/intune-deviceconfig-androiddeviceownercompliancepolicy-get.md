---
title: Получение Андроиддевицеовнеркомплианцеполици
description: Чтение свойств и связей объекта Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12044e34dcf7d7b4971b39689c52a87ba3a8573c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450099"
---
# <a name="get-androiddeviceownercompliancepolicy"></a><span data-ttu-id="fb716-103">Получение Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="fb716-103">Get androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="fb716-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fb716-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb716-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb716-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb716-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb716-107">Чтение свойств и связей объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fb716-107">Read properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb716-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb716-108">Prerequisites</span></span>
<span data-ttu-id="fb716-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb716-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb716-111">Permission type</span></span>|<span data-ttu-id="fb716-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb716-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb716-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb716-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb716-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb716-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb716-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb716-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb716-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb716-116">Not supported.</span></span>|
|<span data-ttu-id="fb716-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb716-117">Application</span></span>|<span data-ttu-id="fb716-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb716-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb716-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb716-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb716-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb716-120">Optional query parameters</span></span>
<span data-ttu-id="fb716-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb716-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb716-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb716-122">Request headers</span></span>
|<span data-ttu-id="fb716-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb716-123">Header</span></span>|<span data-ttu-id="fb716-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fb716-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb716-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb716-125">Authorization</span></span>|<span data-ttu-id="fb716-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb716-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb716-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fb716-127">Accept</span></span>|<span data-ttu-id="fb716-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fb716-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb716-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb716-129">Request body</span></span>
<span data-ttu-id="fb716-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb716-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb716-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb716-131">Response</span></span>
<span data-ttu-id="fb716-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb716-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb716-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fb716-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb716-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb716-134">Request</span></span>
<span data-ttu-id="fb716-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb716-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fb716-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb716-136">Response</span></span>
<span data-ttu-id="fb716-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb716-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "be2464b4-64b4-be24-b464-24beb46424be",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "advancedThreatProtectionRequiredSecurityLevel": "secured",
    "securityRequireSafetyNetAttestationBasicIntegrity": true,
    "securityRequireSafetyNetAttestationCertifiedDevice": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "passwordRequired": true,
    "passwordMinimumLength": 5,
    "passwordMinimumLetterCharacters": 15,
    "passwordMinimumLowerCaseCharacters": 2,
    "passwordMinimumNonLetterCharacters": 2,
    "passwordMinimumNumericCharacters": 0,
    "passwordMinimumSymbolCharacters": 15,
    "passwordMinimumUpperCaseCharacters": 2,
    "passwordRequiredType": "required",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordCountToBlock": 4,
    "storageRequireEncryption": true
  }
}
```





