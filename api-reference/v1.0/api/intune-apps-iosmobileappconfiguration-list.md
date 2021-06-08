---
title: Список iosMobileAppConfigurations
description: Список свойств и связей объектов iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19c705736bdcbe0dcf0ad9e7b4b09b087fc95b77
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757369"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="d9020-103">Список iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="d9020-103">List iosMobileAppConfigurations</span></span>

<span data-ttu-id="d9020-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9020-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9020-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9020-106">Список свойств и связей объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9020-106">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9020-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d9020-107">Prerequisites</span></span>
<span data-ttu-id="d9020-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9020-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9020-110">Permission type</span></span>|<span data-ttu-id="d9020-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9020-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9020-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9020-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9020-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9020-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9020-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9020-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9020-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9020-115">Not supported.</span></span>|
|<span data-ttu-id="d9020-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d9020-116">Application</span></span>|<span data-ttu-id="d9020-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9020-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9020-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9020-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9020-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d9020-119">Request headers</span></span>
|<span data-ttu-id="d9020-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9020-120">Header</span></span>|<span data-ttu-id="d9020-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d9020-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9020-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9020-122">Authorization</span></span>|<span data-ttu-id="d9020-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9020-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9020-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d9020-124">Accept</span></span>|<span data-ttu-id="d9020-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9020-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9020-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9020-126">Request body</span></span>
<span data-ttu-id="d9020-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9020-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9020-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9020-128">Response</span></span>
<span data-ttu-id="d9020-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d9020-129">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9020-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d9020-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9020-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9020-131">Request</span></span>
<span data-ttu-id="d9020-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9020-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="d9020-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9020-133">Response</span></span>
<span data-ttu-id="d9020-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9020-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
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
  ]
}
```




