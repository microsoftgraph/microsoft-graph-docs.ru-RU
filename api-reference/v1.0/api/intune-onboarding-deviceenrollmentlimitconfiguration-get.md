---
title: Получение deviceEnrollmentLimitConfiguration
description: Чтение свойств и связей объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9b12ce490c1e94cca8e50f31dd53ccbd616ea58
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756914"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="9f5fa-103">Получение deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f5fa-103">Get deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="9f5fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f5fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f5fa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f5fa-106">Чтение свойств и связей объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f5fa-106">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f5fa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f5fa-107">Prerequisites</span></span>
<span data-ttu-id="9f5fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f5fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f5fa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f5fa-110">Permission type</span></span>|<span data-ttu-id="9f5fa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f5fa-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f5fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f5fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f5fa-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f5fa-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f5fa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f5fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f5fa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-115">Not supported.</span></span>|
|<span data-ttu-id="9f5fa-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f5fa-116">Application</span></span>|<span data-ttu-id="9f5fa-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f5fa-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f5fa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f5fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f5fa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f5fa-119">Optional query parameters</span></span>
<span data-ttu-id="9f5fa-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f5fa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f5fa-121">Request headers</span></span>
|<span data-ttu-id="9f5fa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f5fa-122">Header</span></span>|<span data-ttu-id="9f5fa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9f5fa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f5fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f5fa-124">Authorization</span></span>|<span data-ttu-id="9f5fa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f5fa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9f5fa-126">Accept</span></span>|<span data-ttu-id="9f5fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9f5fa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f5fa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f5fa-128">Request body</span></span>
<span data-ttu-id="9f5fa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f5fa-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f5fa-130">Response</span></span>
<span data-ttu-id="9f5fa-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f5fa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9f5fa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f5fa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f5fa-133">Request</span></span>
<span data-ttu-id="9f5fa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9f5fa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f5fa-135">Response</span></span>
<span data-ttu-id="9f5fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f5fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




