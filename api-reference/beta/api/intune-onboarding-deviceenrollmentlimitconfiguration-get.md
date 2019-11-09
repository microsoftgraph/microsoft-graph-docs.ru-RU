---
title: Получение deviceEnrollmentLimitConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0942fc94ab8207e38a9f96498f3468cc3b98a9e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086678"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="969e9-103">Получение deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="969e9-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="969e9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="969e9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="969e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="969e9-106">Чтение свойств и связей объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="969e9-106">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="969e9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="969e9-107">Prerequisites</span></span>
<span data-ttu-id="969e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="969e9-110">Permission type</span></span>|<span data-ttu-id="969e9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="969e9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="969e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="969e9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="969e9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="969e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="969e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969e9-115">Not supported.</span></span>|
|<span data-ttu-id="969e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="969e9-116">Application</span></span>|<span data-ttu-id="969e9-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="969e9-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="969e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="969e9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="969e9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="969e9-119">Optional query parameters</span></span>
<span data-ttu-id="969e9-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="969e9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="969e9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="969e9-121">Request headers</span></span>
|<span data-ttu-id="969e9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="969e9-122">Header</span></span>|<span data-ttu-id="969e9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="969e9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969e9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="969e9-124">Authorization</span></span>|<span data-ttu-id="969e9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="969e9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969e9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="969e9-126">Accept</span></span>|<span data-ttu-id="969e9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="969e9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969e9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="969e9-128">Request body</span></span>
<span data-ttu-id="969e9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="969e9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="969e9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="969e9-130">Response</span></span>
<span data-ttu-id="969e9-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="969e9-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969e9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="969e9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="969e9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="969e9-133">Request</span></span>
<span data-ttu-id="969e9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="969e9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="969e9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="969e9-135">Response</span></span>
<span data-ttu-id="969e9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="969e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
    "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "limit": 5
  }
}
```






