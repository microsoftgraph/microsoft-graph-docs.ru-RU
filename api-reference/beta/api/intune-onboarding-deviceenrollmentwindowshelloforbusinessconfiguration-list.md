---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2e7a620b007e1a28c18727bbcbc8e9fcd69dc8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846692"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="294b5-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="294b5-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="294b5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="294b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="294b5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="294b5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="294b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="294b5-107">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="294b5-107">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="294b5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="294b5-108">Prerequisites</span></span>
<span data-ttu-id="294b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="294b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="294b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="294b5-111">Permission type</span></span>|<span data-ttu-id="294b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="294b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="294b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="294b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="294b5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="294b5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="294b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="294b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="294b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294b5-116">Not supported.</span></span>|
|<span data-ttu-id="294b5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="294b5-117">Application</span></span>|<span data-ttu-id="294b5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294b5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="294b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="294b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="294b5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="294b5-120">Request headers</span></span>
|<span data-ttu-id="294b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="294b5-121">Header</span></span>|<span data-ttu-id="294b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="294b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="294b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="294b5-123">Authorization</span></span>|<span data-ttu-id="294b5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="294b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="294b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="294b5-125">Accept</span></span>|<span data-ttu-id="294b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="294b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="294b5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="294b5-127">Request body</span></span>
<span data-ttu-id="294b5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="294b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="294b5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="294b5-129">Response</span></span>
<span data-ttu-id="294b5-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="294b5-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="294b5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="294b5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="294b5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="294b5-132">Request</span></span>
<span data-ttu-id="294b5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="294b5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="294b5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="294b5-134">Response</span></span>
<span data-ttu-id="294b5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="294b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





