---
title: Get windows10CompliancePolicy
description: Чтение свойств и связей объекта windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc543065cf6dba451bb8540f4fe15c6c670c661a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021086"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="f279f-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f279f-103">Get windows10CompliancePolicy</span></span>

<span data-ttu-id="f279f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f279f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f279f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f279f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f279f-106">Чтение свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f279f-106">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f279f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f279f-107">Prerequisites</span></span>
<span data-ttu-id="f279f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f279f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f279f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f279f-110">Permission type</span></span>|<span data-ttu-id="f279f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f279f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f279f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f279f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f279f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f279f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f279f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f279f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f279f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f279f-115">Not supported.</span></span>|
|<span data-ttu-id="f279f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f279f-116">Application</span></span>|<span data-ttu-id="f279f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f279f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f279f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f279f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f279f-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f279f-119">Optional query parameters</span></span>
<span data-ttu-id="f279f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f279f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f279f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f279f-121">Request headers</span></span>
|<span data-ttu-id="f279f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f279f-122">Header</span></span>|<span data-ttu-id="f279f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f279f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f279f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f279f-124">Authorization</span></span>|<span data-ttu-id="f279f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f279f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f279f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f279f-126">Accept</span></span>|<span data-ttu-id="f279f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f279f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f279f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f279f-128">Request body</span></span>
<span data-ttu-id="f279f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f279f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f279f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f279f-130">Response</span></span>
<span data-ttu-id="f279f-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f279f-131">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f279f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f279f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f279f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f279f-133">Request</span></span>
<span data-ttu-id="f279f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f279f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="f279f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f279f-135">Response</span></span>
<span data-ttu-id="f279f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f279f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1197

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
    "storageRequireEncryption": true
  }
}
```









