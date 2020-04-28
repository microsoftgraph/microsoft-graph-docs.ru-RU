---
title: Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c10d241ecd9d124e253a0c06a1b5a29657be3e49
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383672"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="e9645-103">Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9645-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="e9645-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9645-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9645-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9645-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9645-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9645-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9645-107">Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9645-107">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9645-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9645-108">Prerequisites</span></span>
<span data-ttu-id="e9645-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9645-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9645-111">Permission type</span></span>|<span data-ttu-id="e9645-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9645-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9645-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9645-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9645-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9645-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e9645-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9645-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9645-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9645-116">Not supported.</span></span>|
|<span data-ttu-id="e9645-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9645-117">Application</span></span>|<span data-ttu-id="e9645-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9645-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9645-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9645-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9645-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9645-120">Optional query parameters</span></span>
<span data-ttu-id="e9645-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9645-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9645-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9645-122">Request headers</span></span>
|<span data-ttu-id="e9645-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9645-123">Header</span></span>|<span data-ttu-id="e9645-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e9645-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9645-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9645-125">Authorization</span></span>|<span data-ttu-id="e9645-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9645-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9645-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e9645-127">Accept</span></span>|<span data-ttu-id="e9645-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e9645-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9645-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9645-129">Request body</span></span>
<span data-ttu-id="e9645-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9645-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9645-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9645-131">Response</span></span>
<span data-ttu-id="e9645-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9645-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9645-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e9645-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9645-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9645-134">Request</span></span>
<span data-ttu-id="e9645-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9645-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e9645-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9645-136">Response</span></span>
<span data-ttu-id="e9645-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9645-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 900

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
    "enhancedBiometricsState": "enabled",
    "securityKeyForSignIn": "enabled"
  }
}
```



