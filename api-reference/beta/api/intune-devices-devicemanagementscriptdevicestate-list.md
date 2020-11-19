---
title: Список Девицеманажементскриптдевицестатес
description: Список свойств и связей объектов Девицеманажементскриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f93ede247823ccefb4fc5e331835307efe6c948
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212890"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="36a90-103">Список Девицеманажементскриптдевицестатес</span><span class="sxs-lookup"><span data-stu-id="36a90-103">List deviceManagementScriptDeviceStates</span></span>

<span data-ttu-id="36a90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36a90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36a90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36a90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a90-107">Список свойств и связей объектов [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="36a90-107">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36a90-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36a90-108">Prerequisites</span></span>
<span data-ttu-id="36a90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36a90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36a90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36a90-111">Permission type</span></span>|<span data-ttu-id="36a90-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36a90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36a90-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36a90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36a90-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="36a90-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="36a90-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36a90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36a90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a90-116">Not supported.</span></span>|
|<span data-ttu-id="36a90-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="36a90-117">Application</span></span>|<span data-ttu-id="36a90-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="36a90-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36a90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36a90-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="36a90-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36a90-120">Request headers</span></span>
|<span data-ttu-id="36a90-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36a90-121">Header</span></span>|<span data-ttu-id="36a90-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36a90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36a90-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36a90-123">Authorization</span></span>|<span data-ttu-id="36a90-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36a90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36a90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36a90-125">Accept</span></span>|<span data-ttu-id="36a90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36a90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36a90-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36a90-127">Request body</span></span>
<span data-ttu-id="36a90-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36a90-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36a90-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a90-129">Response</span></span>
<span data-ttu-id="36a90-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36a90-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36a90-131">Пример</span><span class="sxs-lookup"><span data-stu-id="36a90-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="36a90-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="36a90-132">Request</span></span>
<span data-ttu-id="36a90-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36a90-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="36a90-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a90-134">Response</span></span>
<span data-ttu-id="36a90-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36a90-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




