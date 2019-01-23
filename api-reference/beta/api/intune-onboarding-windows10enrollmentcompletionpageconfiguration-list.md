---
title: Список windows10EnrollmentCompletionPageConfigurations
description: Свойства списка и связей объектов windows10EnrollmentCompletionPageConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: daa369d9d735ea2cf34f80ca3d9e21bae037e00a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403121"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="2ede3-103">Список windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="2ede3-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="2ede3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ede3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ede3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ede3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ede3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ede3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ede3-107">Свойства списка и связей объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2ede3-107">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ede3-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2ede3-108">Prerequisites</span></span>
<span data-ttu-id="2ede3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ede3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ede3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ede3-111">Permission type</span></span>|<span data-ttu-id="2ede3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ede3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ede3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ede3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ede3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ede3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2ede3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ede3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ede3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ede3-116">Not supported.</span></span>|
|<span data-ttu-id="2ede3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ede3-117">Application</span></span>|<span data-ttu-id="2ede3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ede3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ede3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ede3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2ede3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ede3-120">Request headers</span></span>
|<span data-ttu-id="2ede3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ede3-121">Header</span></span>|<span data-ttu-id="2ede3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ede3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ede3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ede3-123">Authorization</span></span>|<span data-ttu-id="2ede3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2ede3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ede3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ede3-125">Accept</span></span>|<span data-ttu-id="2ede3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ede3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ede3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ede3-127">Request body</span></span>
<span data-ttu-id="2ede3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ede3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ede3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ede3-129">Response</span></span>
<span data-ttu-id="2ede3-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2ede3-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ede3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2ede3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ede3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ede3-132">Request</span></span>
<span data-ttu-id="2ede3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ede3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="2ede3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ede3-134">Response</span></span>
<span data-ttu-id="2ede3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2ede3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
      "id": "77bf8248-8248-77bf-4882-bf774882bf77",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "showInstallationProgress": true,
      "blockDeviceSetupRetryByUser": true,
      "allowDeviceResetOnInstallFailure": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true,
      "selectedMobileAppIds": [
        "Selected Mobile App Ids value"
      ]
    }
  ]
}
```




