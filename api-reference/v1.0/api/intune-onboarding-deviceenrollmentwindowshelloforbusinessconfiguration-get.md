---
title: Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82bd7b709c563535b50a47feafa40bf78ba2cafb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743702"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="ae62f-103">Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae62f-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="ae62f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae62f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae62f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae62f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae62f-106">Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae62f-106">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae62f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ae62f-107">Prerequisites</span></span>
<span data-ttu-id="ae62f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae62f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae62f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae62f-110">Permission type</span></span>|<span data-ttu-id="ae62f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae62f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae62f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae62f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae62f-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae62f-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae62f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae62f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae62f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae62f-115">Not supported.</span></span>|
|<span data-ttu-id="ae62f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae62f-116">Application</span></span>|<span data-ttu-id="ae62f-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae62f-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae62f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae62f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae62f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae62f-119">Optional query parameters</span></span>
<span data-ttu-id="ae62f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae62f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae62f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae62f-121">Request headers</span></span>
|<span data-ttu-id="ae62f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae62f-122">Header</span></span>|<span data-ttu-id="ae62f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ae62f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae62f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae62f-124">Authorization</span></span>|<span data-ttu-id="ae62f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae62f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae62f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ae62f-126">Accept</span></span>|<span data-ttu-id="ae62f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ae62f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae62f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae62f-128">Request body</span></span>
<span data-ttu-id="ae62f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae62f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae62f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae62f-130">Response</span></span>
<span data-ttu-id="ae62f-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ae62f-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae62f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ae62f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae62f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae62f-133">Request</span></span>
<span data-ttu-id="ae62f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae62f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ae62f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae62f-135">Response</span></span>
<span data-ttu-id="ae62f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae62f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
    "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "state": "enabled",
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "remotePassportEnabled": true,
    "pinPreviousBlockCount": 5,
    "pinExpirationInDays": 3,
    "enhancedBiometricsState": "enabled"
  }
}
```




