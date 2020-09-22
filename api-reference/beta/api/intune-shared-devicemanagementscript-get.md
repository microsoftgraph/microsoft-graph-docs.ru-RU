---
title: Получение deviceManagementScript
description: Чтение свойств и связей объекта deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26d0c660d8285491fecbd7372a5018a6cf5d8d20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074330"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="e8bc7-103">Получение deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="e8bc7-103">Get deviceManagementScript</span></span>

<span data-ttu-id="e8bc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8bc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8bc7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8bc7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8bc7-107">Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e8bc7-107">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8bc7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8bc7-108">Prerequisites</span></span>
<span data-ttu-id="e8bc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8bc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8bc7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8bc7-111">Permission type</span></span>|<span data-ttu-id="e8bc7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8bc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8bc7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8bc7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e8bc7-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e8bc7-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e8bc7-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8bc7-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="e8bc7-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="e8bc7-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e8bc7-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8bc7-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e8bc7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8bc7-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8bc7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-119">Not supported.</span></span>|
|<span data-ttu-id="e8bc7-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8bc7-120">Application</span></span>||
| <span data-ttu-id="e8bc7-121">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e8bc7-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e8bc7-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8bc7-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="e8bc7-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="e8bc7-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e8bc7-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8bc7-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8bc7-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8bc7-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8bc7-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8bc7-126">Optional query parameters</span></span>
<span data-ttu-id="e8bc7-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8bc7-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8bc7-128">Request headers</span></span>
|<span data-ttu-id="e8bc7-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8bc7-129">Header</span></span>|<span data-ttu-id="e8bc7-130">Значение</span><span class="sxs-lookup"><span data-stu-id="e8bc7-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8bc7-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8bc7-131">Authorization</span></span>|<span data-ttu-id="e8bc7-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8bc7-133">Accept</span><span class="sxs-lookup"><span data-stu-id="e8bc7-133">Accept</span></span>|<span data-ttu-id="e8bc7-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e8bc7-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8bc7-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8bc7-135">Request body</span></span>
<span data-ttu-id="e8bc7-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8bc7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8bc7-137">Response</span></span>
<span data-ttu-id="e8bc7-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-138">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8bc7-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e8bc7-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8bc7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8bc7-140">Request</span></span>
<span data-ttu-id="e8bc7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="e8bc7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8bc7-142">Response</span></span>
<span data-ttu-id="e8bc7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8bc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": {
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
}
```









