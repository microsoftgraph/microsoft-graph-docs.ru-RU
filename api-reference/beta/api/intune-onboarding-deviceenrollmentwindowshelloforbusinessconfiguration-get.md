---
title: Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a9412a4a84c0768fb8f8047f9987a1b46109f5d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790482"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="12731-103">Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="12731-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="12731-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12731-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12731-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12731-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12731-106">Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12731-106">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12731-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12731-107">Prerequisites</span></span>
<span data-ttu-id="12731-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12731-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12731-110">Permission type</span></span>|<span data-ttu-id="12731-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12731-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12731-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12731-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12731-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="12731-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="12731-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12731-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12731-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12731-115">Not supported.</span></span>|
|<span data-ttu-id="12731-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12731-116">Application</span></span>|<span data-ttu-id="12731-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12731-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12731-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12731-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12731-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12731-119">Optional query parameters</span></span>
<span data-ttu-id="12731-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12731-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12731-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12731-121">Request headers</span></span>
|<span data-ttu-id="12731-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12731-122">Header</span></span>|<span data-ttu-id="12731-123">Значение</span><span class="sxs-lookup"><span data-stu-id="12731-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12731-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12731-124">Authorization</span></span>|<span data-ttu-id="12731-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12731-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12731-126">Accept</span><span class="sxs-lookup"><span data-stu-id="12731-126">Accept</span></span>|<span data-ttu-id="12731-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12731-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12731-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12731-128">Request body</span></span>
<span data-ttu-id="12731-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12731-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12731-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="12731-130">Response</span></span>
<span data-ttu-id="12731-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12731-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12731-132">Пример</span><span class="sxs-lookup"><span data-stu-id="12731-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="12731-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="12731-133">Request</span></span>
<span data-ttu-id="12731-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12731-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="12731-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="12731-135">Response</span></span>
<span data-ttu-id="12731-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12731-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





