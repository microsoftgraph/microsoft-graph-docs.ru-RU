---
title: Получение deviceManagementScript
description: Чтение свойств и связей объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50bb84f7bb216bca9367f1e6129c6d6c4525e11a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201046"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="6ba24-103">Получение deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="6ba24-103">Get deviceManagementScript</span></span>

> <span data-ttu-id="6ba24-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ba24-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ba24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ba24-106">Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="6ba24-106">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ba24-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ba24-107">Prerequisites</span></span>
<span data-ttu-id="6ba24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ba24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ba24-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ba24-110">Permission type</span></span>|<span data-ttu-id="6ba24-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ba24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ba24-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ba24-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6ba24-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6ba24-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6ba24-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ba24-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6ba24-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6ba24-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6ba24-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ba24-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6ba24-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ba24-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ba24-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba24-118">Not supported.</span></span>|
|<span data-ttu-id="6ba24-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ba24-119">Application</span></span>||
| <span data-ttu-id="6ba24-120">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6ba24-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6ba24-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ba24-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6ba24-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6ba24-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6ba24-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ba24-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ba24-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ba24-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ba24-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ba24-125">Optional query parameters</span></span>
<span data-ttu-id="6ba24-126">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ba24-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ba24-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ba24-127">Request headers</span></span>
|<span data-ttu-id="6ba24-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ba24-128">Header</span></span>|<span data-ttu-id="6ba24-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6ba24-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ba24-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ba24-130">Authorization</span></span>|<span data-ttu-id="6ba24-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ba24-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ba24-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6ba24-132">Accept</span></span>|<span data-ttu-id="6ba24-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6ba24-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ba24-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ba24-134">Request body</span></span>
<span data-ttu-id="6ba24-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ba24-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ba24-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ba24-136">Response</span></span>
<span data-ttu-id="6ba24-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ba24-137">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ba24-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6ba24-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ba24-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ba24-139">Request</span></span>
<span data-ttu-id="6ba24-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ba24-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="6ba24-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ba24-141">Response</span></span>
<span data-ttu-id="6ba24-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ba24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




