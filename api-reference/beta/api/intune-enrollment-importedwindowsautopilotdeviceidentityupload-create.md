---
title: Создание Импортедвиндовсаутопилотдевицеидентитюплоад
description: Создание нового объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f9da24beab9076f01d18864aa9fe4a648bef902
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959889"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="d5f39-103">Создание Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="d5f39-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="d5f39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5f39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5f39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5f39-106">Создание нового объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f39-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5f39-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5f39-107">Prerequisites</span></span>
<span data-ttu-id="d5f39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5f39-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f39-110">Permission type</span></span>|<span data-ttu-id="d5f39-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5f39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5f39-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5f39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5f39-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5f39-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5f39-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5f39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5f39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f39-115">Not supported.</span></span>|
|<span data-ttu-id="d5f39-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5f39-116">Application</span></span>|<span data-ttu-id="d5f39-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5f39-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5f39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="d5f39-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5f39-119">Request headers</span></span>
|<span data-ttu-id="d5f39-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5f39-120">Header</span></span>|<span data-ttu-id="d5f39-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d5f39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5f39-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5f39-122">Authorization</span></span>|<span data-ttu-id="d5f39-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5f39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5f39-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d5f39-124">Accept</span></span>|<span data-ttu-id="d5f39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5f39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5f39-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5f39-126">Request body</span></span>
<span data-ttu-id="d5f39-127">В тексте запроса добавьте представление объекта Импортедвиндовсаутопилотдевицеидентитюплоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5f39-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="d5f39-128">В следующей таблице приведены свойства, необходимые при создании Импортедвиндовсаутопилотдевицеидентитюплоад.</span><span class="sxs-lookup"><span data-stu-id="d5f39-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="d5f39-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5f39-129">Property</span></span>|<span data-ttu-id="d5f39-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d5f39-130">Type</span></span>|<span data-ttu-id="d5f39-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d5f39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5f39-132">id</span><span class="sxs-lookup"><span data-stu-id="d5f39-132">id</span></span>|<span data-ttu-id="d5f39-133">String</span><span class="sxs-lookup"><span data-stu-id="d5f39-133">String</span></span>|<span data-ttu-id="d5f39-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="d5f39-134">The GUID for the object</span></span>|
|<span data-ttu-id="d5f39-135">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="d5f39-135">createdDateTimeUtc</span></span>|<span data-ttu-id="d5f39-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f39-136">DateTimeOffset</span></span>|<span data-ttu-id="d5f39-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d5f39-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="d5f39-138">status</span><span class="sxs-lookup"><span data-stu-id="d5f39-138">status</span></span>|[<span data-ttu-id="d5f39-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="d5f39-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="d5f39-140">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d5f39-140">Upload status.</span></span> <span data-ttu-id="d5f39-141">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="d5f39-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="d5f39-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5f39-142">Response</span></span>
<span data-ttu-id="d5f39-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5f39-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5f39-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d5f39-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5f39-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5f39-145">Request</span></span>
<span data-ttu-id="d5f39-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5f39-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="d5f39-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5f39-147">Response</span></span>
<span data-ttu-id="d5f39-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5f39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




