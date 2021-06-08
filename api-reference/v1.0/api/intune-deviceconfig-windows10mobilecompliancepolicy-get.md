---
title: Get windows10MobileCompliancePolicy
description: Чтение свойств и связей объекта windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b90b17e5da691e39de76e6ef8ac3147dc5c589f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760505"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="7ecc0-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7ecc0-103">Get windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="7ecc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ecc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ecc0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ecc0-106">Чтение свойств и связей объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ecc0-106">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ecc0-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7ecc0-107">Prerequisites</span></span>
<span data-ttu-id="7ecc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ecc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ecc0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ecc0-110">Permission type</span></span>|<span data-ttu-id="7ecc0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ecc0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ecc0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ecc0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ecc0-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecc0-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ecc0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ecc0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ecc0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-115">Not supported.</span></span>|
|<span data-ttu-id="7ecc0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ecc0-116">Application</span></span>|<span data-ttu-id="7ecc0-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ecc0-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ecc0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ecc0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ecc0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ecc0-119">Optional query parameters</span></span>
<span data-ttu-id="7ecc0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ecc0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ecc0-121">Request headers</span></span>
|<span data-ttu-id="7ecc0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ecc0-122">Header</span></span>|<span data-ttu-id="7ecc0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7ecc0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ecc0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ecc0-124">Authorization</span></span>|<span data-ttu-id="7ecc0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ecc0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7ecc0-126">Accept</span></span>|<span data-ttu-id="7ecc0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7ecc0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ecc0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ecc0-128">Request body</span></span>
<span data-ttu-id="7ecc0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ecc0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ecc0-130">Response</span></span>
<span data-ttu-id="7ecc0-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-131">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ecc0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7ecc0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ecc0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ecc0-133">Request</span></span>
<span data-ttu-id="7ecc0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="7ecc0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ecc0-135">Response</span></span>
<span data-ttu-id="7ecc0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ecc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1029

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
    "storageRequireEncryption": true
  }
}
```




