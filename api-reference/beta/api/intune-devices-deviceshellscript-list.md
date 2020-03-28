---
title: Список Девицешеллскриптс
description: Список свойств и связей объектов Девицешеллскрипт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29bf5a6046318912252b3896b43178f0741c9c1c
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034743"
---
# <a name="list-deviceshellscripts"></a><span data-ttu-id="8e523-103">Список Девицешеллскриптс</span><span class="sxs-lookup"><span data-stu-id="8e523-103">List deviceShellScripts</span></span>

> <span data-ttu-id="8e523-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e523-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e523-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e523-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e523-106">Список свойств и связей объектов [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="8e523-106">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e523-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e523-107">Prerequisites</span></span>
<span data-ttu-id="8e523-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e523-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e523-110">Permission type</span></span>|<span data-ttu-id="8e523-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e523-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e523-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e523-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e523-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e523-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8e523-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e523-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e523-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e523-115">Not supported.</span></span>|
|<span data-ttu-id="8e523-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e523-116">Application</span></span>|<span data-ttu-id="8e523-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e523-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e523-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e523-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="8e523-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8e523-119">Request headers</span></span>
|<span data-ttu-id="8e523-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e523-120">Header</span></span>|<span data-ttu-id="8e523-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8e523-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e523-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e523-122">Authorization</span></span>|<span data-ttu-id="8e523-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e523-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e523-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8e523-124">Accept</span></span>|<span data-ttu-id="8e523-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e523-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e523-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e523-126">Request body</span></span>
<span data-ttu-id="8e523-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e523-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e523-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e523-128">Response</span></span>
<span data-ttu-id="8e523-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e523-129">If successful, this method returns a `200 OK` response code and a collection of [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e523-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8e523-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e523-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e523-131">Request</span></span>
<span data-ttu-id="8e523-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e523-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
```

### <a name="response"></a><span data-ttu-id="8e523-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e523-133">Response</span></span>
<span data-ttu-id="8e523-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e523-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "value": [
    {
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
  ]
}
```



