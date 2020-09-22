---
title: Get androidCustomConfiguration
description: Чтение свойств и связей объекта androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10a75e6d671e8ac91f73d5a6ce085eade92eb354
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985519"
---
# <a name="get-androidcustomconfiguration"></a><span data-ttu-id="3fef0-103">Get androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3fef0-103">Get androidCustomConfiguration</span></span>

<span data-ttu-id="3fef0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fef0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fef0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fef0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fef0-106">Чтение свойств и связей объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3fef0-106">Read properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fef0-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3fef0-107">Prerequisites</span></span>
<span data-ttu-id="3fef0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fef0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fef0-110">Permission type</span></span>|<span data-ttu-id="3fef0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fef0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fef0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fef0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fef0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fef0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3fef0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fef0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fef0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fef0-115">Not supported.</span></span>|
|<span data-ttu-id="3fef0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fef0-116">Application</span></span>|<span data-ttu-id="3fef0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fef0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fef0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fef0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fef0-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3fef0-119">Optional query parameters</span></span>
<span data-ttu-id="3fef0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3fef0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fef0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fef0-121">Request headers</span></span>
|<span data-ttu-id="3fef0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fef0-122">Header</span></span>|<span data-ttu-id="3fef0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3fef0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fef0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fef0-124">Authorization</span></span>|<span data-ttu-id="3fef0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fef0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fef0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3fef0-126">Accept</span></span>|<span data-ttu-id="3fef0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3fef0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fef0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fef0-128">Request body</span></span>
<span data-ttu-id="3fef0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fef0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fef0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fef0-130">Response</span></span>
<span data-ttu-id="3fef0-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3fef0-131">If successful, this method returns a `200 OK` response code and [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fef0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3fef0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fef0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fef0-133">Request</span></span>
<span data-ttu-id="3fef0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fef0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3fef0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fef0-135">Response</span></span>
<span data-ttu-id="3fef0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fef0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 625

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCustomConfiguration",
    "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```









