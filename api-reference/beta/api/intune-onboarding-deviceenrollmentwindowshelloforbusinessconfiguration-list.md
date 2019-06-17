---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1964e86f8229a236d339d17bf279ce2eebf726d2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981120"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="d5def-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5def-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="d5def-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5def-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5def-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5def-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5def-106">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5def-106">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5def-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5def-107">Prerequisites</span></span>
<span data-ttu-id="d5def-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5def-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5def-110">Permission type</span></span>|<span data-ttu-id="d5def-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5def-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5def-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5def-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5def-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5def-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d5def-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5def-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5def-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5def-115">Not supported.</span></span>|
|<span data-ttu-id="d5def-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5def-116">Application</span></span>|<span data-ttu-id="d5def-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5def-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5def-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5def-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5def-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5def-119">Request headers</span></span>
|<span data-ttu-id="d5def-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5def-120">Header</span></span>|<span data-ttu-id="d5def-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d5def-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5def-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5def-122">Authorization</span></span>|<span data-ttu-id="d5def-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5def-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5def-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d5def-124">Accept</span></span>|<span data-ttu-id="d5def-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5def-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5def-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5def-126">Request body</span></span>
<span data-ttu-id="d5def-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5def-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5def-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5def-128">Response</span></span>
<span data-ttu-id="d5def-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5def-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5def-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d5def-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5def-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5def-131">Request</span></span>
<span data-ttu-id="d5def-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5def-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="d5def-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5def-133">Response</span></span>
<span data-ttu-id="d5def-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5def-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 956

{
  "value": [
    {
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
  ]
}
```





