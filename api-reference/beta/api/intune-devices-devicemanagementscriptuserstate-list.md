---
title: Список Девицеманажементскриптусерстатес
description: Список свойств и связей объектов Девицеманажементскриптусерстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d7d5462e1420db5bbf9a5935dbab1308a399572
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708244"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="60772-103">Список Девицеманажементскриптусерстатес</span><span class="sxs-lookup"><span data-stu-id="60772-103">List deviceManagementScriptUserStates</span></span>

<span data-ttu-id="60772-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60772-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60772-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60772-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60772-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60772-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60772-107">Список свойств и связей объектов [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="60772-107">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60772-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="60772-108">Prerequisites</span></span>
<span data-ttu-id="60772-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60772-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60772-111">Permission type</span></span>|<span data-ttu-id="60772-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="60772-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60772-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60772-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60772-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="60772-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="60772-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60772-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60772-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60772-116">Not supported.</span></span>|
|<span data-ttu-id="60772-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60772-117">Application</span></span>|<span data-ttu-id="60772-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="60772-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60772-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60772-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="60772-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="60772-120">Request headers</span></span>
|<span data-ttu-id="60772-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60772-121">Header</span></span>|<span data-ttu-id="60772-122">Значение</span><span class="sxs-lookup"><span data-stu-id="60772-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60772-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60772-123">Authorization</span></span>|<span data-ttu-id="60772-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60772-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60772-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60772-125">Accept</span></span>|<span data-ttu-id="60772-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60772-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60772-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60772-127">Request body</span></span>
<span data-ttu-id="60772-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60772-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60772-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="60772-129">Response</span></span>
<span data-ttu-id="60772-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60772-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60772-131">Пример</span><span class="sxs-lookup"><span data-stu-id="60772-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="60772-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="60772-132">Request</span></span>
<span data-ttu-id="60772-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60772-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="60772-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="60772-134">Response</span></span>
<span data-ttu-id="60772-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60772-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
      "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
      "successDeviceCount": 2,
      "errorDeviceCount": 0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





