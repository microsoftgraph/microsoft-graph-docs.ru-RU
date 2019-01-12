---
title: Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Список свойств и связей объектов deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e8162e698996058fd620a2aab0bdc16edf6eb88a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925240"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="21525-103">Перечисление объектов deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="21525-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="21525-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21525-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21525-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21525-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21525-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21525-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21525-107">Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21525-107">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21525-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21525-108">Prerequisites</span></span>
<span data-ttu-id="21525-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21525-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21525-111">Permission type</span></span>|<span data-ttu-id="21525-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21525-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21525-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21525-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21525-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="21525-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="21525-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21525-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21525-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21525-116">Not supported.</span></span>|
|<span data-ttu-id="21525-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21525-117">Application</span></span>|<span data-ttu-id="21525-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21525-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21525-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21525-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="21525-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21525-120">Request headers</span></span>
|<span data-ttu-id="21525-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21525-121">Header</span></span>|<span data-ttu-id="21525-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21525-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21525-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21525-123">Authorization</span></span>|<span data-ttu-id="21525-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21525-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21525-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21525-125">Accept</span></span>|<span data-ttu-id="21525-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21525-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21525-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21525-127">Request body</span></span>
<span data-ttu-id="21525-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21525-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21525-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="21525-129">Response</span></span>
<span data-ttu-id="21525-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21525-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21525-131">Пример</span><span class="sxs-lookup"><span data-stu-id="21525-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="21525-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="21525-132">Request</span></span>
<span data-ttu-id="21525-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21525-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="21525-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="21525-134">Response</span></span>
<span data-ttu-id="21525-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21525-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





