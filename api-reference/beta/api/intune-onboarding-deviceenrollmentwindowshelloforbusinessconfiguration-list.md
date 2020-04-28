---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b46207c56f1601efdc1b979a457525b0420e70d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469562"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="cf8fc-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf8fc-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

<span data-ttu-id="cf8fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf8fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf8fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf8fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf8fc-107">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf8fc-107">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf8fc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cf8fc-108">Prerequisites</span></span>
<span data-ttu-id="cf8fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf8fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf8fc-111">Permission type</span></span>|<span data-ttu-id="cf8fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf8fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf8fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf8fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf8fc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf8fc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cf8fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf8fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf8fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-116">Not supported.</span></span>|
|<span data-ttu-id="cf8fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf8fc-117">Application</span></span>|<span data-ttu-id="cf8fc-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf8fc-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf8fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf8fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cf8fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf8fc-120">Request headers</span></span>
|<span data-ttu-id="cf8fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf8fc-121">Header</span></span>|<span data-ttu-id="cf8fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf8fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf8fc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf8fc-123">Authorization</span></span>|<span data-ttu-id="cf8fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf8fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf8fc-125">Accept</span></span>|<span data-ttu-id="cf8fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf8fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf8fc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf8fc-127">Request body</span></span>
<span data-ttu-id="cf8fc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf8fc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf8fc-129">Response</span></span>
<span data-ttu-id="cf8fc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf8fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cf8fc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf8fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf8fc-132">Request</span></span>
<span data-ttu-id="cf8fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="cf8fc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf8fc-134">Response</span></span>
<span data-ttu-id="cf8fc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf8fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



