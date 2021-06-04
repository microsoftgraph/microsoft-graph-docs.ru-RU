---
title: Перечисление объектов deviceConfiguration
description: Список свойств и связей объектов deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61f3be260aa95c35e6655339aa2912d88db853c3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753935"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="17a20-103">Перечисление объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="17a20-103">List deviceConfigurations</span></span>

<span data-ttu-id="17a20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17a20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17a20-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17a20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17a20-106">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17a20-106">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17a20-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17a20-107">Prerequisites</span></span>
<span data-ttu-id="17a20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17a20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17a20-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17a20-110">Permission type</span></span>|<span data-ttu-id="17a20-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17a20-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17a20-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17a20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17a20-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a20-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17a20-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17a20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17a20-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17a20-115">Not supported.</span></span>|
|<span data-ttu-id="17a20-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="17a20-116">Application</span></span>|<span data-ttu-id="17a20-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a20-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17a20-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17a20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="17a20-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17a20-119">Request headers</span></span>
|<span data-ttu-id="17a20-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17a20-120">Header</span></span>|<span data-ttu-id="17a20-121">Значение</span><span class="sxs-lookup"><span data-stu-id="17a20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17a20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17a20-122">Authorization</span></span>|<span data-ttu-id="17a20-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17a20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17a20-124">Accept</span><span class="sxs-lookup"><span data-stu-id="17a20-124">Accept</span></span>|<span data-ttu-id="17a20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17a20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17a20-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17a20-126">Request body</span></span>
<span data-ttu-id="17a20-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17a20-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17a20-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="17a20-128">Response</span></span>
<span data-ttu-id="17a20-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17a20-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17a20-130">Пример</span><span class="sxs-lookup"><span data-stu-id="17a20-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="17a20-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="17a20-131">Request</span></span>
<span data-ttu-id="17a20-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17a20-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="17a20-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="17a20-133">Response</span></span>
<span data-ttu-id="17a20-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17a20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfiguration",
      "id": "34977265-7265-3497-6572-973465729734",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




