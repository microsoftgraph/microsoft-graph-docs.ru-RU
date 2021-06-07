---
title: Получить iosMobileAppConfiguration
description: Чтение списка свойств и связей объекта iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b240b9856a9efa7aaa24a070c4249c44871cfc63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757376"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="833d0-103">Получить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="833d0-103">Get iosMobileAppConfiguration</span></span>

<span data-ttu-id="833d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="833d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="833d0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="833d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="833d0-106">Чтение списка свойств и связей объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="833d0-106">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="833d0-107">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="833d0-107">Prerequisites</span></span>
<span data-ttu-id="833d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="833d0-110">Permission type</span></span>|<span data-ttu-id="833d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="833d0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="833d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="833d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="833d0-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833d0-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="833d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="833d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="833d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833d0-115">Not supported.</span></span>|
|<span data-ttu-id="833d0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="833d0-116">Application</span></span>|<span data-ttu-id="833d0-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833d0-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="833d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="833d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="833d0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="833d0-119">Optional query parameters</span></span>
<span data-ttu-id="833d0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="833d0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="833d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="833d0-121">Request headers</span></span>
|<span data-ttu-id="833d0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="833d0-122">Header</span></span>|<span data-ttu-id="833d0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="833d0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="833d0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="833d0-124">Authorization</span></span>|<span data-ttu-id="833d0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="833d0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="833d0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="833d0-126">Accept</span></span>|<span data-ttu-id="833d0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="833d0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="833d0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="833d0-128">Request body</span></span>
<span data-ttu-id="833d0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="833d0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="833d0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="833d0-130">Response</span></span>
<span data-ttu-id="833d0-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="833d0-131">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="833d0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="833d0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="833d0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="833d0-133">Request</span></span>
<span data-ttu-id="833d0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="833d0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="833d0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="833d0-135">Response</span></span>
<span data-ttu-id="833d0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="833d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```




