---
title: Get windows10SecureAssessmentConfiguration
description: Чтение свойств и связей объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d8d98338a52dfa593bb16a6030c8a9752544ad5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760463"
---
# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="1dbf9-103">Get windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="1dbf9-103">Get windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="1dbf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dbf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dbf9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dbf9-106">Чтение свойств и связей объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbf9-106">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dbf9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1dbf9-107">Prerequisites</span></span>
<span data-ttu-id="1dbf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dbf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dbf9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dbf9-110">Permission type</span></span>|<span data-ttu-id="1dbf9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dbf9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dbf9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dbf9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dbf9-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbf9-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1dbf9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dbf9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dbf9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-115">Not supported.</span></span>|
|<span data-ttu-id="1dbf9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1dbf9-116">Application</span></span>|<span data-ttu-id="1dbf9-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbf9-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dbf9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dbf9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1dbf9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1dbf9-119">Optional query parameters</span></span>
<span data-ttu-id="1dbf9-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dbf9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dbf9-121">Request headers</span></span>
|<span data-ttu-id="1dbf9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dbf9-122">Header</span></span>|<span data-ttu-id="1dbf9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1dbf9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dbf9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dbf9-124">Authorization</span></span>|<span data-ttu-id="1dbf9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dbf9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1dbf9-126">Accept</span></span>|<span data-ttu-id="1dbf9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1dbf9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbf9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dbf9-128">Request body</span></span>
<span data-ttu-id="1dbf9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dbf9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbf9-130">Response</span></span>
<span data-ttu-id="1dbf9-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-131">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dbf9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1dbf9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dbf9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dbf9-133">Request</span></span>
<span data-ttu-id="1dbf9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1dbf9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbf9-135">Response</span></span>
<span data-ttu-id="1dbf9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dbf9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
    "id": "f60d71be-71be-f60d-be71-0df6be710df6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "launchUri": "Launch Uri value",
    "configurationAccount": "Configuration Account value",
    "allowPrinting": true,
    "allowScreenCapture": true,
    "allowTextSuggestion": true
  }
}
```




