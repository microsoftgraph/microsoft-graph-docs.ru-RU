---
title: Обновление Импортедвиндовсаутопилотдевицеидентитюплоад
description: Обновление свойств объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 867561d9c361cbc725b6223d08d51002680d82f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985577"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="3975f-103">Обновление Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="3975f-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="3975f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3975f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3975f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3975f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3975f-106">Обновление свойств объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="3975f-106">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3975f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3975f-107">Prerequisites</span></span>
<span data-ttu-id="3975f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3975f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3975f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3975f-110">Permission type</span></span>|<span data-ttu-id="3975f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3975f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3975f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3975f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3975f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3975f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3975f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3975f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3975f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3975f-115">Not supported.</span></span>|
|<span data-ttu-id="3975f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3975f-116">Application</span></span>|<span data-ttu-id="3975f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3975f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3975f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3975f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="3975f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3975f-119">Request headers</span></span>
|<span data-ttu-id="3975f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3975f-120">Header</span></span>|<span data-ttu-id="3975f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3975f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3975f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3975f-122">Authorization</span></span>|<span data-ttu-id="3975f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3975f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3975f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3975f-124">Accept</span></span>|<span data-ttu-id="3975f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3975f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3975f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3975f-126">Request body</span></span>
<span data-ttu-id="3975f-127">В тексте запроса добавьте представление объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3975f-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="3975f-128">В следующей таблице приведены свойства, необходимые при создании [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="3975f-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="3975f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3975f-129">Property</span></span>|<span data-ttu-id="3975f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3975f-130">Type</span></span>|<span data-ttu-id="3975f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3975f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3975f-132">id</span><span class="sxs-lookup"><span data-stu-id="3975f-132">id</span></span>|<span data-ttu-id="3975f-133">String</span><span class="sxs-lookup"><span data-stu-id="3975f-133">String</span></span>|<span data-ttu-id="3975f-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="3975f-134">The GUID for the object</span></span>|
|<span data-ttu-id="3975f-135">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="3975f-135">createdDateTimeUtc</span></span>|<span data-ttu-id="3975f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3975f-136">DateTimeOffset</span></span>|<span data-ttu-id="3975f-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3975f-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="3975f-138">status</span><span class="sxs-lookup"><span data-stu-id="3975f-138">status</span></span>|[<span data-ttu-id="3975f-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="3975f-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="3975f-140">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3975f-140">Upload status.</span></span> <span data-ttu-id="3975f-141">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="3975f-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="3975f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3975f-142">Response</span></span>
<span data-ttu-id="3975f-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3975f-143">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3975f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3975f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3975f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3975f-145">Request</span></span>
<span data-ttu-id="3975f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3975f-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="3975f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3975f-147">Response</span></span>
<span data-ttu-id="3975f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3975f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```





