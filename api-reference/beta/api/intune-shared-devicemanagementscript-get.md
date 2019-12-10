---
title: Получение deviceManagementScript
description: Чтение свойств и связей объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6cb673aa19737483d6151267f579493a96561372
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939895"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="0fbda-103">Получение deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0fbda-103">Get deviceManagementScript</span></span>

> <span data-ttu-id="0fbda-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fbda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fbda-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fbda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbda-106">Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0fbda-106">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fbda-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0fbda-107">Prerequisites</span></span>
<span data-ttu-id="0fbda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fbda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fbda-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fbda-110">Permission type</span></span>|<span data-ttu-id="0fbda-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fbda-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fbda-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fbda-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0fbda-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0fbda-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0fbda-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbda-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="0fbda-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="0fbda-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0fbda-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbda-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0fbda-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fbda-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fbda-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fbda-118">Not supported.</span></span>|
|<span data-ttu-id="0fbda-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fbda-119">Application</span></span>||
| <span data-ttu-id="0fbda-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0fbda-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0fbda-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbda-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="0fbda-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="0fbda-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0fbda-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbda-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fbda-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fbda-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fbda-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0fbda-125">Optional query parameters</span></span>
<span data-ttu-id="0fbda-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0fbda-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fbda-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fbda-127">Request headers</span></span>
|<span data-ttu-id="0fbda-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fbda-128">Header</span></span>|<span data-ttu-id="0fbda-129">Значение</span><span class="sxs-lookup"><span data-stu-id="0fbda-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fbda-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fbda-130">Authorization</span></span>|<span data-ttu-id="0fbda-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fbda-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fbda-132">Accept</span><span class="sxs-lookup"><span data-stu-id="0fbda-132">Accept</span></span>|<span data-ttu-id="0fbda-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0fbda-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fbda-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fbda-134">Request body</span></span>
<span data-ttu-id="0fbda-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fbda-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fbda-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fbda-136">Response</span></span>
<span data-ttu-id="0fbda-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fbda-137">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fbda-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0fbda-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fbda-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fbda-139">Request</span></span>
<span data-ttu-id="0fbda-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fbda-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="0fbda-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fbda-141">Response</span></span>
<span data-ttu-id="0fbda-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fbda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








