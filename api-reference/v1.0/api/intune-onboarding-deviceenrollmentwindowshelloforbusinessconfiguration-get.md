---
title: Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4a0ce40baa3a7275b870b920617d73a061c408e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561490"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="e1c57-103">Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1c57-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="e1c57-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1c57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1c57-105">Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c57-105">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1c57-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e1c57-106">Prerequisites</span></span>
<span data-ttu-id="e1c57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1c57-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1c57-109">Permission type</span></span>|<span data-ttu-id="e1c57-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1c57-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1c57-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1c57-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1c57-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1c57-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e1c57-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1c57-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1c57-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c57-114">Not supported.</span></span>|
|<span data-ttu-id="e1c57-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1c57-115">Application</span></span>|<span data-ttu-id="e1c57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c57-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1c57-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1c57-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1c57-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1c57-118">Optional query parameters</span></span>
<span data-ttu-id="e1c57-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1c57-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1c57-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1c57-120">Request headers</span></span>
|<span data-ttu-id="e1c57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1c57-121">Header</span></span>|<span data-ttu-id="e1c57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1c57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1c57-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1c57-123">Authorization</span></span>|<span data-ttu-id="e1c57-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1c57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1c57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1c57-125">Accept</span></span>|<span data-ttu-id="e1c57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1c57-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1c57-127">Request body</span></span>
<span data-ttu-id="e1c57-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1c57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1c57-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c57-129">Response</span></span>
<span data-ttu-id="e1c57-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1c57-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1c57-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e1c57-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1c57-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1c57-132">Request</span></span>
<span data-ttu-id="e1c57-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1c57-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1c57-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c57-134">Response</span></span>
<span data-ttu-id="e1c57-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1c57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



