---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52b3dd4633b6be115de8a0c2d1d38a216f75b3c9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725684"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="660df-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="660df-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

<span data-ttu-id="660df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="660df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="660df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="660df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="660df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="660df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="660df-107">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="660df-107">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="660df-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="660df-108">Prerequisites</span></span>
<span data-ttu-id="660df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="660df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="660df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="660df-111">Permission type</span></span>|<span data-ttu-id="660df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="660df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="660df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="660df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="660df-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="660df-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="660df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="660df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="660df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="660df-116">Not supported.</span></span>|
|<span data-ttu-id="660df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="660df-117">Application</span></span>|<span data-ttu-id="660df-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="660df-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="660df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="660df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="660df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="660df-120">Request headers</span></span>
|<span data-ttu-id="660df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="660df-121">Header</span></span>|<span data-ttu-id="660df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="660df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="660df-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="660df-123">Authorization</span></span>|<span data-ttu-id="660df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="660df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="660df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="660df-125">Accept</span></span>|<span data-ttu-id="660df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="660df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="660df-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="660df-127">Request body</span></span>
<span data-ttu-id="660df-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="660df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="660df-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="660df-129">Response</span></span>
<span data-ttu-id="660df-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="660df-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="660df-131">Пример</span><span class="sxs-lookup"><span data-stu-id="660df-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="660df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="660df-132">Request</span></span>
<span data-ttu-id="660df-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="660df-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="660df-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="660df-134">Response</span></span>
<span data-ttu-id="660df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="660df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1030

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
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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





