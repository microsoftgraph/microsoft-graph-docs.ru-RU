---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 217877475cfedb7b920ee48f8e5604a2958cc648
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025797"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="f80ed-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f80ed-103">List targetedManagedAppConfigurations</span></span>

<span data-ttu-id="f80ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f80ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f80ed-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f80ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f80ed-106">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f80ed-106">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f80ed-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f80ed-107">Prerequisites</span></span>
<span data-ttu-id="f80ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f80ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f80ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f80ed-110">Permission type</span></span>|<span data-ttu-id="f80ed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f80ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f80ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f80ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f80ed-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f80ed-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f80ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f80ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f80ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f80ed-115">Not supported.</span></span>|
|<span data-ttu-id="f80ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f80ed-116">Application</span></span>|<span data-ttu-id="f80ed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f80ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f80ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f80ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f80ed-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f80ed-119">Request headers</span></span>
|<span data-ttu-id="f80ed-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f80ed-120">Header</span></span>|<span data-ttu-id="f80ed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f80ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f80ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f80ed-122">Authorization</span></span>|<span data-ttu-id="f80ed-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f80ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f80ed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f80ed-124">Accept</span></span>|<span data-ttu-id="f80ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f80ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f80ed-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f80ed-126">Request body</span></span>
<span data-ttu-id="f80ed-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f80ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f80ed-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f80ed-128">Response</span></span>
<span data-ttu-id="f80ed-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f80ed-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f80ed-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f80ed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f80ed-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f80ed-131">Request</span></span>
<span data-ttu-id="f80ed-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f80ed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="f80ed-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f80ed-133">Response</span></span>
<span data-ttu-id="f80ed-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f80ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```









