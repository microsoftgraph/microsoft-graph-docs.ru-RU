---
title: Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03d9957f1c51132c74cdc4b190d5770370cf1e63
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252163"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="f7ea5-103">Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7ea5-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="f7ea5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ea5-105">Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7ea5-105">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7ea5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7ea5-106">Prerequisites</span></span>
<span data-ttu-id="f7ea5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7ea5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7ea5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7ea5-109">Permission type</span></span>|<span data-ttu-id="f7ea5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7ea5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7ea5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7ea5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7ea5-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7ea5-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f7ea5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7ea5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7ea5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-114">Not supported.</span></span>|
|<span data-ttu-id="f7ea5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7ea5-115">Application</span></span>|<span data-ttu-id="f7ea5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7ea5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7ea5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7ea5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7ea5-118">Optional query parameters</span></span>
<span data-ttu-id="f7ea5-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7ea5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7ea5-120">Request headers</span></span>
|<span data-ttu-id="f7ea5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7ea5-121">Header</span></span>|<span data-ttu-id="f7ea5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7ea5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7ea5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7ea5-123">Authorization</span></span>|<span data-ttu-id="f7ea5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7ea5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7ea5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7ea5-125">Accept</span></span>|<span data-ttu-id="f7ea5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7ea5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7ea5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7ea5-127">Request body</span></span>
<span data-ttu-id="f7ea5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7ea5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7ea5-129">Response</span></span>
<span data-ttu-id="f7ea5-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ea5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f7ea5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7ea5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7ea5-132">Request</span></span>
<span data-ttu-id="f7ea5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f7ea5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7ea5-134">Response</span></span>
<span data-ttu-id="f7ea5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7ea5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



