---
title: Получение Девицешеллскрипт
description: Чтение свойств и связей объекта Девицешеллскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b16eea0e21cb579eb0bac78cf7f06fd6e4ceac49
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994633"
---
# <a name="get-deviceshellscript"></a><span data-ttu-id="9c324-103">Получение Девицешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="9c324-103">Get deviceShellScript</span></span>

<span data-ttu-id="9c324-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c324-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c324-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c324-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c324-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c324-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c324-107">Чтение свойств и связей объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="9c324-107">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c324-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c324-108">Prerequisites</span></span>
<span data-ttu-id="9c324-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c324-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c324-111">Permission type</span></span>|<span data-ttu-id="9c324-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c324-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c324-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c324-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c324-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9c324-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c324-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c324-116">Not supported.</span></span>|
|<span data-ttu-id="9c324-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c324-117">Application</span></span>|<span data-ttu-id="9c324-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c324-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c324-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c324-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="9c324-120">Optional query parameters</span></span>
<span data-ttu-id="9c324-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9c324-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c324-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c324-122">Request headers</span></span>
|<span data-ttu-id="9c324-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c324-123">Header</span></span>|<span data-ttu-id="9c324-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9c324-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c324-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c324-125">Authorization</span></span>|<span data-ttu-id="9c324-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c324-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c324-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9c324-127">Accept</span></span>|<span data-ttu-id="9c324-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9c324-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c324-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c324-129">Request body</span></span>
<span data-ttu-id="9c324-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c324-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c324-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c324-131">Response</span></span>
<span data-ttu-id="9c324-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c324-132">If successful, this method returns a `200 OK` response code and [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c324-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9c324-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c324-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c324-134">Request</span></span>
<span data-ttu-id="9c324-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c324-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

### <a name="response"></a><span data-ttu-id="9c324-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c324-136">Response</span></span>
<span data-ttu-id="9c324-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c324-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceShellScript",
    "executionFrequency": "PT2M43.444327S",
    "retryCount": 10,
    "blockExecutionNotifications": true,
    "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
    "displayName": "Display Name value",
    "description": "Description value",
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "fileName": "File Name value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






