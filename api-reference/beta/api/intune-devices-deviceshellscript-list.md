---
title: Список устройствShellScripts
description: Список свойств и связей объектов deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8ae0af64decbc3e13a9d51dc857c39a679bb58e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150250"
---
# <a name="list-deviceshellscripts"></a><span data-ttu-id="ba695-103">Список устройствShellScripts</span><span class="sxs-lookup"><span data-stu-id="ba695-103">List deviceShellScripts</span></span>

<span data-ttu-id="ba695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba695-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba695-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba695-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba695-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba695-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba695-107">Список свойств и связей объектов [deviceShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="ba695-107">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba695-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba695-108">Prerequisites</span></span>
<span data-ttu-id="ba695-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba695-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba695-111">Permission type</span></span>|<span data-ttu-id="ba695-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba695-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba695-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba695-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba695-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba695-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ba695-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba695-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba695-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba695-116">Not supported.</span></span>|
|<span data-ttu-id="ba695-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba695-117">Application</span></span>|<span data-ttu-id="ba695-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba695-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba695-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba695-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="ba695-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba695-120">Request headers</span></span>
|<span data-ttu-id="ba695-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba695-121">Header</span></span>|<span data-ttu-id="ba695-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba695-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba695-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba695-123">Authorization</span></span>|<span data-ttu-id="ba695-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba695-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba695-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba695-125">Accept</span></span>|<span data-ttu-id="ba695-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba695-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba695-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba695-127">Request body</span></span>
<span data-ttu-id="ba695-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba695-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba695-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba695-129">Response</span></span>
<span data-ttu-id="ba695-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceShellScript](../resources/intune-devices-deviceshellscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ba695-130">If successful, this method returns a `200 OK` response code and a collection of [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba695-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ba695-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba695-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba695-132">Request</span></span>
<span data-ttu-id="ba695-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba695-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
```

### <a name="response"></a><span data-ttu-id="ba695-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba695-134">Response</span></span>
<span data-ttu-id="ba695-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba695-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




