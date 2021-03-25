---
title: Список deviceManagementScriptDeviceStates
description: Список свойств и связей объектов deviceManagementScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1bf8b516681fceac43ad0d1fd56dbfac7b72852
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150446"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="afe22-103">Список deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="afe22-103">List deviceManagementScriptDeviceStates</span></span>

<span data-ttu-id="afe22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afe22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afe22-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afe22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afe22-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="afe22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afe22-107">Список свойств и связей [объектов deviceManagementScriptDeviceState.](../resources/intune-devices-devicemanagementscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="afe22-107">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afe22-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="afe22-108">Prerequisites</span></span>
<span data-ttu-id="afe22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe22-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afe22-111">Permission type</span></span>|<span data-ttu-id="afe22-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afe22-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afe22-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afe22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afe22-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe22-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="afe22-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afe22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afe22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afe22-116">Not supported.</span></span>|
|<span data-ttu-id="afe22-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="afe22-117">Application</span></span>|<span data-ttu-id="afe22-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe22-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afe22-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afe22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="afe22-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="afe22-120">Request headers</span></span>
|<span data-ttu-id="afe22-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="afe22-121">Header</span></span>|<span data-ttu-id="afe22-122">Значение</span><span class="sxs-lookup"><span data-stu-id="afe22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afe22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afe22-123">Authorization</span></span>|<span data-ttu-id="afe22-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afe22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afe22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="afe22-125">Accept</span></span>|<span data-ttu-id="afe22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afe22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afe22-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afe22-127">Request body</span></span>
<span data-ttu-id="afe22-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afe22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afe22-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="afe22-129">Response</span></span>
<span data-ttu-id="afe22-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="afe22-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afe22-131">Пример</span><span class="sxs-lookup"><span data-stu-id="afe22-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="afe22-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="afe22-132">Request</span></span>
<span data-ttu-id="afe22-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afe22-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="afe22-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="afe22-134">Response</span></span>
<span data-ttu-id="afe22-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afe22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value"
    }
  ]
}
```




