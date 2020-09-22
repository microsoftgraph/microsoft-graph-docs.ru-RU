---
title: Список importedWindowsAutopilotDeviceIdentityUploads
description: Список свойств и связей объектов Импортедвиндовсаутопилотдевицеидентитюплоад.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3a13de39cacf4a6e37c792a85491bcc9cebbf28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979016"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="7e241-103">Список importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="7e241-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

<span data-ttu-id="7e241-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e241-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e241-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e241-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e241-106">Список свойств и связей объектов [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="7e241-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e241-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e241-107">Prerequisites</span></span>
<span data-ttu-id="7e241-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e241-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e241-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e241-110">Permission type</span></span>|<span data-ttu-id="7e241-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e241-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e241-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e241-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e241-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e241-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7e241-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e241-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e241-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e241-115">Not supported.</span></span>|
|<span data-ttu-id="7e241-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e241-116">Application</span></span>|<span data-ttu-id="7e241-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e241-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e241-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e241-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="7e241-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e241-119">Request headers</span></span>
|<span data-ttu-id="7e241-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e241-120">Header</span></span>|<span data-ttu-id="7e241-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7e241-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e241-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e241-122">Authorization</span></span>|<span data-ttu-id="7e241-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e241-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e241-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7e241-124">Accept</span></span>|<span data-ttu-id="7e241-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e241-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e241-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e241-126">Request body</span></span>
<span data-ttu-id="7e241-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e241-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e241-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e241-128">Response</span></span>
<span data-ttu-id="7e241-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e241-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e241-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7e241-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e241-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e241-131">Request</span></span>
<span data-ttu-id="7e241-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e241-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="7e241-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e241-133">Response</span></span>
<span data-ttu-id="7e241-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e241-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```









