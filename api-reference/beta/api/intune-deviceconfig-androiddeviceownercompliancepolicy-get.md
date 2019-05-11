---
title: Получение Андроиддевицеовнеркомплианцеполици
description: Чтение свойств и связей объекта Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd8750fb70bae08cc4d0103a5cd65cac0b9a2e2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933272"
---
# <a name="get-androiddeviceownercompliancepolicy"></a><span data-ttu-id="8d278-103">Получение Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="8d278-103">Get androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="8d278-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d278-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d278-106">Чтение свойств и связей объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8d278-106">Read properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d278-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d278-107">Prerequisites</span></span>
<span data-ttu-id="8d278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d278-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d278-110">Permission type</span></span>|<span data-ttu-id="8d278-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d278-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d278-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d278-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d278-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d278-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d278-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d278-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d278-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d278-115">Not supported.</span></span>|
|<span data-ttu-id="8d278-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d278-116">Application</span></span>|<span data-ttu-id="8d278-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d278-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d278-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d278-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d278-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d278-119">Optional query parameters</span></span>
<span data-ttu-id="8d278-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d278-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d278-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d278-121">Request headers</span></span>
|<span data-ttu-id="8d278-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d278-122">Header</span></span>|<span data-ttu-id="8d278-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8d278-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d278-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d278-124">Authorization</span></span>|<span data-ttu-id="8d278-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d278-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d278-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8d278-126">Accept</span></span>|<span data-ttu-id="8d278-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8d278-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d278-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d278-128">Request body</span></span>
<span data-ttu-id="8d278-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d278-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d278-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d278-130">Response</span></span>
<span data-ttu-id="8d278-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d278-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d278-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8d278-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d278-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d278-133">Request</span></span>
<span data-ttu-id="8d278-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d278-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="8d278-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d278-135">Response</span></span>
<span data-ttu-id="8d278-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d278-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1175

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




