---
title: Список windows10EnrollmentCompletionPageConfigurations
description: Свойства списка и связей объектов windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ec24ae93a913e943706ed26a190cdb10c9bb10db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877156"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="b8d92-103">Список windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="b8d92-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="b8d92-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8d92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8d92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8d92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8d92-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8d92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8d92-107">Свойства списка и связей объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b8d92-107">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8d92-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8d92-108">Prerequisites</span></span>
<span data-ttu-id="b8d92-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8d92-111">Permission type</span></span>|<span data-ttu-id="b8d92-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8d92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8d92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8d92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8d92-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d92-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b8d92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8d92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8d92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8d92-116">Not supported.</span></span>|
|<span data-ttu-id="b8d92-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8d92-117">Application</span></span>|<span data-ttu-id="b8d92-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8d92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8d92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8d92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8d92-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8d92-120">Request headers</span></span>
|<span data-ttu-id="b8d92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8d92-121">Header</span></span>|<span data-ttu-id="b8d92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8d92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8d92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d92-123">Authorization</span></span>|<span data-ttu-id="b8d92-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b8d92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8d92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8d92-125">Accept</span></span>|<span data-ttu-id="b8d92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8d92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8d92-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8d92-127">Request body</span></span>
<span data-ttu-id="b8d92-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8d92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8d92-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8d92-129">Response</span></span>
<span data-ttu-id="b8d92-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b8d92-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d92-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b8d92-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8d92-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8d92-132">Request</span></span>
<span data-ttu-id="b8d92-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8d92-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b8d92-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8d92-134">Response</span></span>
<span data-ttu-id="b8d92-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b8d92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





