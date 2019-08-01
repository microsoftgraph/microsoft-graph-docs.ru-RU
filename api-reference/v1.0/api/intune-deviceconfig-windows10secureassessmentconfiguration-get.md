---
title: Get windows10SecureAssessmentConfiguration
description: Чтение свойств и связей объекта windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc3030116f5c6274dd60dca24d309ca1c759071a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020110"
---
# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="c1b0b-103">Get windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1b0b-103">Get windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="c1b0b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1b0b-105">Чтение свойств и связей объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1b0b-105">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1b0b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b0b-106">Prerequisites</span></span>
<span data-ttu-id="c1b0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1b0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b0b-109">Permission type</span></span>|<span data-ttu-id="c1b0b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1b0b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1b0b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b0b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1b0b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c1b0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1b0b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-114">Not supported.</span></span>|
|<span data-ttu-id="c1b0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1b0b-115">Application</span></span>|<span data-ttu-id="c1b0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1b0b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1b0b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1b0b-118">Optional query parameters</span></span>
<span data-ttu-id="c1b0b-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1b0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1b0b-120">Request headers</span></span>
|<span data-ttu-id="c1b0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1b0b-121">Header</span></span>|<span data-ttu-id="c1b0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1b0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1b0b-123">Authorization</span></span>|<span data-ttu-id="c1b0b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1b0b-125">Accept</span></span>|<span data-ttu-id="c1b0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b0b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1b0b-127">Request body</span></span>
<span data-ttu-id="c1b0b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1b0b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1b0b-129">Response</span></span>
<span data-ttu-id="c1b0b-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-130">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b0b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c1b0b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1b0b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1b0b-132">Request</span></span>
<span data-ttu-id="c1b0b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c1b0b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b0b-134">Response</span></span>
<span data-ttu-id="c1b0b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1b0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



