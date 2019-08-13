---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de92d6ba615b72e3dc5bc13a591cedd6ed25719f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352877"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="b0308-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0308-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="b0308-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0308-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0308-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0308-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0308-106">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0308-106">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0308-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0308-107">Prerequisites</span></span>
<span data-ttu-id="b0308-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0308-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0308-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0308-110">Permission type</span></span>|<span data-ttu-id="b0308-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0308-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0308-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0308-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0308-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0308-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b0308-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0308-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0308-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0308-115">Not supported.</span></span>|
|<span data-ttu-id="b0308-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0308-116">Application</span></span>|<span data-ttu-id="b0308-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0308-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0308-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0308-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0308-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0308-119">Request headers</span></span>
|<span data-ttu-id="b0308-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0308-120">Header</span></span>|<span data-ttu-id="b0308-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0308-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0308-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0308-122">Authorization</span></span>|<span data-ttu-id="b0308-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0308-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0308-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b0308-124">Accept</span></span>|<span data-ttu-id="b0308-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0308-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0308-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0308-126">Request body</span></span>
<span data-ttu-id="b0308-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0308-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0308-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0308-128">Response</span></span>
<span data-ttu-id="b0308-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0308-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0308-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b0308-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0308-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0308-131">Request</span></span>
<span data-ttu-id="b0308-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0308-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b0308-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0308-133">Response</span></span>
<span data-ttu-id="b0308-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0308-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






