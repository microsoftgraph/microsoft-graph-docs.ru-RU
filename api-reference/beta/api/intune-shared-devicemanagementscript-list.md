---
title: Список deviceManagementScripts
description: Список свойств и связей объектов deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e352f7a594550bcebd4592ef79692fae491a9765
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692802"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="58977-103">Список deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="58977-103">List deviceManagementScripts</span></span>

<span data-ttu-id="58977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58977-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58977-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58977-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58977-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58977-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58977-107">Список свойств и связей объектов [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="58977-107">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58977-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58977-108">Prerequisites</span></span>
<span data-ttu-id="58977-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58977-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58977-111">Permission type</span></span>|<span data-ttu-id="58977-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58977-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58977-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58977-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="58977-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="58977-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="58977-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58977-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="58977-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="58977-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="58977-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58977-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="58977-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58977-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58977-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58977-119">Not supported.</span></span>|
|<span data-ttu-id="58977-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58977-120">Application</span></span>||
| <span data-ttu-id="58977-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="58977-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="58977-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58977-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="58977-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="58977-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="58977-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58977-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58977-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58977-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="58977-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58977-126">Request headers</span></span>
|<span data-ttu-id="58977-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58977-127">Header</span></span>|<span data-ttu-id="58977-128">Значение</span><span class="sxs-lookup"><span data-stu-id="58977-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58977-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58977-129">Authorization</span></span>|<span data-ttu-id="58977-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58977-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58977-131">Accept</span><span class="sxs-lookup"><span data-stu-id="58977-131">Accept</span></span>|<span data-ttu-id="58977-132">application/json</span><span class="sxs-lookup"><span data-stu-id="58977-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58977-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58977-133">Request body</span></span>
<span data-ttu-id="58977-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58977-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58977-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="58977-135">Response</span></span>
<span data-ttu-id="58977-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58977-136">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58977-137">Пример</span><span class="sxs-lookup"><span data-stu-id="58977-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="58977-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="58977-138">Request</span></span>
<span data-ttu-id="58977-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58977-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="58977-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="58977-140">Response</span></span>
<span data-ttu-id="58977-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58977-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








