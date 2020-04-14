---
title: Перечисление объектов detectedApp
description: Список свойств и связей объектов detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8540d4ec02071a01cebd799d73250dcf5426bf7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381004"
---
# <a name="list-detectedapps"></a><span data-ttu-id="f0648-103">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="f0648-103">List detectedApps</span></span>

<span data-ttu-id="f0648-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0648-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0648-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0648-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0648-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0648-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0648-107">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0648-107">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0648-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0648-108">Prerequisites</span></span>
<span data-ttu-id="f0648-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0648-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0648-111">Permission type</span></span>|<span data-ttu-id="f0648-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0648-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0648-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0648-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0648-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0648-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f0648-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0648-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0648-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0648-116">Not supported.</span></span>|
|<span data-ttu-id="f0648-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f0648-117">Application</span></span>|<span data-ttu-id="f0648-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0648-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0648-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0648-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="f0648-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0648-120">Request headers</span></span>
|<span data-ttu-id="f0648-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0648-121">Header</span></span>|<span data-ttu-id="f0648-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0648-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0648-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0648-123">Authorization</span></span>|<span data-ttu-id="f0648-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0648-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0648-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0648-125">Accept</span></span>|<span data-ttu-id="f0648-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0648-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0648-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0648-127">Request body</span></span>
<span data-ttu-id="f0648-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0648-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0648-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0648-129">Response</span></span>
<span data-ttu-id="f0648-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [detectedApp](../resources/intune-devices-detectedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0648-130">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0648-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f0648-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0648-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0648-132">Request</span></span>
<span data-ttu-id="f0648-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0648-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="f0648-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0648-134">Response</span></span>
<span data-ttu-id="f0648-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0648-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```



