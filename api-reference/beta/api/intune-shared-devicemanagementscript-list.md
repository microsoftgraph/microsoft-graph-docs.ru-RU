---
title: Список deviceManagementScripts
description: Список свойств и связей объектов deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d131ef8f0ba69a1e799d62fb7ab64932f3c0db1
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085957"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="27ab6-103">Список deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="27ab6-103">List deviceManagementScripts</span></span>

> <span data-ttu-id="27ab6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27ab6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27ab6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27ab6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27ab6-106">Список свойств и связей объектов [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="27ab6-106">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27ab6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27ab6-107">Prerequisites</span></span>
<span data-ttu-id="27ab6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27ab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27ab6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27ab6-110">Permission type</span></span>|<span data-ttu-id="27ab6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27ab6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27ab6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27ab6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="27ab6-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="27ab6-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="27ab6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="27ab6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="27ab6-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="27ab6-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="27ab6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="27ab6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="27ab6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27ab6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27ab6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27ab6-118">Not supported.</span></span>|
|<span data-ttu-id="27ab6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27ab6-119">Application</span></span>||
| <span data-ttu-id="27ab6-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="27ab6-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="27ab6-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="27ab6-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="27ab6-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="27ab6-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="27ab6-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="27ab6-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27ab6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27ab6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="27ab6-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="27ab6-125">Request headers</span></span>
|<span data-ttu-id="27ab6-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27ab6-126">Header</span></span>|<span data-ttu-id="27ab6-127">Значение</span><span class="sxs-lookup"><span data-stu-id="27ab6-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27ab6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27ab6-128">Authorization</span></span>|<span data-ttu-id="27ab6-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27ab6-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27ab6-130">Accept</span><span class="sxs-lookup"><span data-stu-id="27ab6-130">Accept</span></span>|<span data-ttu-id="27ab6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="27ab6-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27ab6-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27ab6-132">Request body</span></span>
<span data-ttu-id="27ab6-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27ab6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27ab6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="27ab6-134">Response</span></span>
<span data-ttu-id="27ab6-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27ab6-135">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27ab6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="27ab6-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="27ab6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="27ab6-137">Request</span></span>
<span data-ttu-id="27ab6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27ab6-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="27ab6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="27ab6-139">Response</span></span>
<span data-ttu-id="27ab6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27ab6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScript",
      "id": "59ea4525-4525-59ea-2545-ea592545ea59",
      "displayName": "Display Name value",
      "description": "Description value",
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      },
      "scriptContent": "c2NyaXB0Q29udGVudA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "fileName": "File Name value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "runAs32Bit": true
    }
  ]
}
```









