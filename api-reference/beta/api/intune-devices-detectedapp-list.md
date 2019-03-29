---
title: Перечисление объектов detectedApp
description: Список свойств и связей объектов detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a786161c209dddb4fc244870f704755ddd07f4e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965055"
---
# <a name="list-detectedapps"></a><span data-ttu-id="54d33-103">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="54d33-103">List detectedApps</span></span>

> <span data-ttu-id="54d33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54d33-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54d33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54d33-106">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="54d33-106">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54d33-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="54d33-107">Prerequisites</span></span>
<span data-ttu-id="54d33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54d33-110">Permission type</span></span>|<span data-ttu-id="54d33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54d33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54d33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54d33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54d33-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="54d33-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="54d33-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54d33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54d33-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d33-115">Not supported.</span></span>|
|<span data-ttu-id="54d33-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54d33-116">Application</span></span>|<span data-ttu-id="54d33-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54d33-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54d33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="54d33-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54d33-119">Request headers</span></span>
|<span data-ttu-id="54d33-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54d33-120">Header</span></span>|<span data-ttu-id="54d33-121">Значение</span><span class="sxs-lookup"><span data-stu-id="54d33-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54d33-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54d33-122">Authorization</span></span>|<span data-ttu-id="54d33-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54d33-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54d33-124">Accept</span><span class="sxs-lookup"><span data-stu-id="54d33-124">Accept</span></span>|<span data-ttu-id="54d33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54d33-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54d33-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54d33-126">Request body</span></span>
<span data-ttu-id="54d33-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54d33-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d33-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="54d33-128">Response</span></span>
<span data-ttu-id="54d33-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [detectedApp](../resources/intune-devices-detectedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54d33-129">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d33-130">Пример</span><span class="sxs-lookup"><span data-stu-id="54d33-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="54d33-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="54d33-131">Request</span></span>
<span data-ttu-id="54d33-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54d33-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="54d33-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="54d33-133">Response</span></span>
<span data-ttu-id="54d33-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54d33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




