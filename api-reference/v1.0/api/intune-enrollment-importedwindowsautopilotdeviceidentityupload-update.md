---
title: Обновление Импортедвиндовсаутопилотдевицеидентитюплоад
description: Обновление свойств объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5bd613884d06fb3b5d10172c71873d4276238a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020803"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="2e512-103">Обновление Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="2e512-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="2e512-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e512-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e512-105">Обновление свойств объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="2e512-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e512-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e512-106">Prerequisites</span></span>
<span data-ttu-id="2e512-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e512-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e512-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e512-109">Permission type</span></span>|<span data-ttu-id="2e512-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e512-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e512-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e512-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e512-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e512-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e512-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e512-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e512-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e512-114">Not supported.</span></span>|
|<span data-ttu-id="2e512-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e512-115">Application</span></span>|<span data-ttu-id="2e512-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e512-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e512-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e512-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="2e512-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e512-118">Request headers</span></span>
|<span data-ttu-id="2e512-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e512-119">Header</span></span>|<span data-ttu-id="2e512-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2e512-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e512-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e512-121">Authorization</span></span>|<span data-ttu-id="2e512-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e512-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e512-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2e512-123">Accept</span></span>|<span data-ttu-id="2e512-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e512-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e512-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e512-125">Request body</span></span>
<span data-ttu-id="2e512-126">В тексте запроса добавьте представление объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e512-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="2e512-127">В следующей таблице приведены свойства, необходимые при создании [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="2e512-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="2e512-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e512-128">Property</span></span>|<span data-ttu-id="2e512-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2e512-129">Type</span></span>|<span data-ttu-id="2e512-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2e512-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e512-131">id</span><span class="sxs-lookup"><span data-stu-id="2e512-131">id</span></span>|<span data-ttu-id="2e512-132">String</span><span class="sxs-lookup"><span data-stu-id="2e512-132">String</span></span>|<span data-ttu-id="2e512-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="2e512-133">The GUID for the object</span></span>|
|<span data-ttu-id="2e512-134">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="2e512-134">createdDateTimeUtc</span></span>|<span data-ttu-id="2e512-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e512-135">DateTimeOffset</span></span>|<span data-ttu-id="2e512-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2e512-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="2e512-137">status</span><span class="sxs-lookup"><span data-stu-id="2e512-137">status</span></span>|[<span data-ttu-id="2e512-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="2e512-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="2e512-139">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="2e512-139">Upload status.</span></span> <span data-ttu-id="2e512-140">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="2e512-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e512-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e512-141">Response</span></span>
<span data-ttu-id="2e512-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e512-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e512-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2e512-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e512-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e512-144">Request</span></span>
<span data-ttu-id="2e512-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e512-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="2e512-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e512-146">Response</span></span>
<span data-ttu-id="2e512-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e512-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



