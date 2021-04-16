---
title: Список deviceManagementScripts
description: Список свойств и связей объектов deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 056f8c012ba31322f0afcc824f3fab67fe681c65
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867751"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="1bdf6-103">Список deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="1bdf6-103">List deviceManagementScripts</span></span>

<span data-ttu-id="1bdf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bdf6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bdf6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bdf6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bdf6-107">Список свойств и связей объектов [deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="1bdf6-107">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bdf6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1bdf6-108">Prerequisites</span></span>
<span data-ttu-id="1bdf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bdf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdf6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdf6-111">Permission type</span></span>|<span data-ttu-id="1bdf6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bdf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdf6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bdf6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1bdf6-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="1bdf6-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1bdf6-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdf6-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="1bdf6-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="1bdf6-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1bdf6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdf6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1bdf6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bdf6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdf6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-119">Not supported.</span></span>|
|<span data-ttu-id="1bdf6-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1bdf6-120">Application</span></span>||
| <span data-ttu-id="1bdf6-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="1bdf6-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1bdf6-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdf6-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="1bdf6-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="1bdf6-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1bdf6-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdf6-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdf6-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bdf6-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="1bdf6-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1bdf6-126">Request headers</span></span>
|<span data-ttu-id="1bdf6-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bdf6-127">Header</span></span>|<span data-ttu-id="1bdf6-128">Значение</span><span class="sxs-lookup"><span data-stu-id="1bdf6-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdf6-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bdf6-129">Authorization</span></span>|<span data-ttu-id="1bdf6-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdf6-131">Accept</span><span class="sxs-lookup"><span data-stu-id="1bdf6-131">Accept</span></span>|<span data-ttu-id="1bdf6-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdf6-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdf6-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bdf6-133">Request body</span></span>
<span data-ttu-id="1bdf6-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bdf6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdf6-135">Response</span></span>
<span data-ttu-id="1bdf6-136">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-136">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdf6-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1bdf6-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bdf6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bdf6-138">Request</span></span>
<span data-ttu-id="1bdf6-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="1bdf6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdf6-140">Response</span></span>
<span data-ttu-id="1bdf6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bdf6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







