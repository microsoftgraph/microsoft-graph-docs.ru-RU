---
title: Создание Импортедвиндовсаутопилотдевицеидентитюплоад
description: Создание нового объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f263379b2e94515b0c49f7c6cfdb7a3b9d525ff8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513387"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="5988a-103">Создание Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="5988a-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

<span data-ttu-id="5988a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5988a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5988a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5988a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5988a-106">Создание нового объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="5988a-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5988a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5988a-107">Prerequisites</span></span>
<span data-ttu-id="5988a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5988a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5988a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5988a-110">Permission type</span></span>|<span data-ttu-id="5988a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5988a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5988a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5988a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5988a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5988a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5988a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5988a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5988a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5988a-115">Not supported.</span></span>|
|<span data-ttu-id="5988a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5988a-116">Application</span></span>|<span data-ttu-id="5988a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5988a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5988a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5988a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="5988a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5988a-119">Request headers</span></span>
|<span data-ttu-id="5988a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5988a-120">Header</span></span>|<span data-ttu-id="5988a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5988a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5988a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5988a-122">Authorization</span></span>|<span data-ttu-id="5988a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5988a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5988a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5988a-124">Accept</span></span>|<span data-ttu-id="5988a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5988a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5988a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5988a-126">Request body</span></span>
<span data-ttu-id="5988a-127">В тексте запроса добавьте представление объекта Импортедвиндовсаутопилотдевицеидентитюплоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5988a-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="5988a-128">В следующей таблице приведены свойства, необходимые при создании Импортедвиндовсаутопилотдевицеидентитюплоад.</span><span class="sxs-lookup"><span data-stu-id="5988a-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="5988a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5988a-129">Property</span></span>|<span data-ttu-id="5988a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5988a-130">Type</span></span>|<span data-ttu-id="5988a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5988a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5988a-132">id</span><span class="sxs-lookup"><span data-stu-id="5988a-132">id</span></span>|<span data-ttu-id="5988a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5988a-133">String</span></span>|<span data-ttu-id="5988a-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="5988a-134">The GUID for the object</span></span>|
|<span data-ttu-id="5988a-135">креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="5988a-135">createdDateTimeUtc</span></span>|<span data-ttu-id="5988a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5988a-136">DateTimeOffset</span></span>|<span data-ttu-id="5988a-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5988a-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="5988a-138">status</span><span class="sxs-lookup"><span data-stu-id="5988a-138">status</span></span>|[<span data-ttu-id="5988a-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="5988a-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="5988a-140">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="5988a-140">Upload status.</span></span> <span data-ttu-id="5988a-141">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="5988a-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="5988a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5988a-142">Response</span></span>
<span data-ttu-id="5988a-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5988a-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5988a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5988a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5988a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5988a-145">Request</span></span>
<span data-ttu-id="5988a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5988a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="5988a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5988a-147">Response</span></span>
<span data-ttu-id="5988a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5988a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```




