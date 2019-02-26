---
title: Список windows10EnrollmentCompletionPageConfigurations
description: Список свойств и связей объектов windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef07ce0c3f37d2ac27c74557d10e2a697adac644
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154756"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="e09cb-103">Список windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="e09cb-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="e09cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e09cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e09cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e09cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e09cb-106">Список свойств и связей объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e09cb-106">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e09cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e09cb-107">Prerequisites</span></span>
<span data-ttu-id="e09cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e09cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e09cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e09cb-110">Permission type</span></span>|<span data-ttu-id="e09cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e09cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e09cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e09cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e09cb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e09cb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e09cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e09cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e09cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e09cb-115">Not supported.</span></span>|
|<span data-ttu-id="e09cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e09cb-116">Application</span></span>|<span data-ttu-id="e09cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e09cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e09cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e09cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e09cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e09cb-119">Request headers</span></span>
|<span data-ttu-id="e09cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e09cb-120">Header</span></span>|<span data-ttu-id="e09cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e09cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e09cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e09cb-122">Authorization</span></span>|<span data-ttu-id="e09cb-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e09cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e09cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e09cb-124">Accept</span></span>|<span data-ttu-id="e09cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e09cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e09cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e09cb-126">Request body</span></span>
<span data-ttu-id="e09cb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e09cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e09cb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e09cb-128">Response</span></span>
<span data-ttu-id="e09cb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e09cb-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e09cb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e09cb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e09cb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e09cb-131">Request</span></span>
<span data-ttu-id="e09cb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e09cb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="e09cb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e09cb-133">Response</span></span>
<span data-ttu-id="e09cb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e09cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




