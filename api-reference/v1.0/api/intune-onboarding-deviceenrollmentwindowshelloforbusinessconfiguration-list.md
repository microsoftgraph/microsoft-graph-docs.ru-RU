---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53d8f984862cede4a00a97af5536d76dbef38b56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989136"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="677d9-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="677d9-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="677d9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="677d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="677d9-105">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="677d9-105">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="677d9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="677d9-106">Prerequisites</span></span>
<span data-ttu-id="677d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="677d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="677d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="677d9-109">Permission type</span></span>|<span data-ttu-id="677d9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="677d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="677d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="677d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="677d9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="677d9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="677d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="677d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="677d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677d9-114">Not supported.</span></span>|
|<span data-ttu-id="677d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="677d9-115">Application</span></span>|<span data-ttu-id="677d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="677d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="677d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="677d9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="677d9-118">Request headers</span></span>
|<span data-ttu-id="677d9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="677d9-119">Header</span></span>|<span data-ttu-id="677d9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="677d9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="677d9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="677d9-121">Authorization</span></span>|<span data-ttu-id="677d9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="677d9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="677d9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="677d9-123">Accept</span></span>|<span data-ttu-id="677d9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="677d9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="677d9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="677d9-125">Request body</span></span>
<span data-ttu-id="677d9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="677d9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="677d9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="677d9-127">Response</span></span>
<span data-ttu-id="677d9-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="677d9-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="677d9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="677d9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="677d9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="677d9-130">Request</span></span>
<span data-ttu-id="677d9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="677d9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="677d9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="677d9-132">Response</span></span>
<span data-ttu-id="677d9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="677d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

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
      "enhancedBiometricsState": "enabled"
    }
  ]
}
```



