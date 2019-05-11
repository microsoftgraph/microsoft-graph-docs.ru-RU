---
title: Список importedWindowsAutopilotDeviceIdentityUploads
description: Список свойств и связей объектов Импортедвиндовсаутопилотдевицеидентитюплоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e637423328fe890c05b75baa669a180a3e34f9ac
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909192"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="6ae3b-103">Список importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="6ae3b-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="6ae3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ae3b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ae3b-106">Список свойств и связей объектов [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="6ae3b-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ae3b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ae3b-107">Prerequisites</span></span>
<span data-ttu-id="6ae3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ae3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ae3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ae3b-110">Permission type</span></span>|<span data-ttu-id="6ae3b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ae3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ae3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ae3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ae3b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ae3b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6ae3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ae3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ae3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-115">Not supported.</span></span>|
|<span data-ttu-id="6ae3b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ae3b-116">Application</span></span>|<span data-ttu-id="6ae3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ae3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ae3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="6ae3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ae3b-119">Request headers</span></span>
|<span data-ttu-id="6ae3b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ae3b-120">Header</span></span>|<span data-ttu-id="6ae3b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ae3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ae3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ae3b-122">Authorization</span></span>|<span data-ttu-id="6ae3b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ae3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ae3b-124">Accept</span></span>|<span data-ttu-id="6ae3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ae3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ae3b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ae3b-126">Request body</span></span>
<span data-ttu-id="6ae3b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ae3b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ae3b-128">Response</span></span>
<span data-ttu-id="6ae3b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ae3b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6ae3b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ae3b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ae3b-131">Request</span></span>
<span data-ttu-id="6ae3b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="6ae3b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ae3b-133">Response</span></span>
<span data-ttu-id="6ae3b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ae3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




