---
title: Перечисление объектов managedDeviceMobileAppConfiguration
description: Перечисление свойств и связей объектов managedDeviceMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe0642f9cbe0c3fd93128b27619bb73930fb5a15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013323"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="5b034-103">Перечисление объектов managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b034-103">List managedDeviceMobileAppConfigurations</span></span>

<span data-ttu-id="5b034-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b034-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b034-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b034-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b034-106">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b034-106">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b034-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b034-107">Prerequisites</span></span>
<span data-ttu-id="5b034-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b034-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b034-110">Permission type</span></span>|<span data-ttu-id="5b034-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b034-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b034-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b034-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b034-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b034-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b034-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b034-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b034-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b034-115">Not supported.</span></span>|
|<span data-ttu-id="5b034-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b034-116">Application</span></span>|<span data-ttu-id="5b034-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b034-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b034-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b034-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5b034-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b034-119">Request headers</span></span>
|<span data-ttu-id="5b034-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b034-120">Header</span></span>|<span data-ttu-id="5b034-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b034-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b034-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b034-122">Authorization</span></span>|<span data-ttu-id="5b034-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b034-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b034-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b034-124">Accept</span></span>|<span data-ttu-id="5b034-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b034-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b034-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b034-126">Request body</span></span>
<span data-ttu-id="5b034-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b034-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b034-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b034-128">Response</span></span>
<span data-ttu-id="5b034-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b034-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b034-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5b034-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b034-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b034-131">Request</span></span>
<span data-ttu-id="5b034-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b034-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="5b034-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b034-133">Response</span></span>
<span data-ttu-id="5b034-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b034-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
      "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```









