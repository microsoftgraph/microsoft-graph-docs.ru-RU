---
title: Создание Импортедвиндовсаутопилотдевицеидентитюплоад
description: Создание нового объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa8e18a8635be0a8955b3e2c7400a5884cf8d3c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532459"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="783ea-103">Создание Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="783ea-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="783ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="783ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="783ea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="783ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="783ea-106">Создание нового объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="783ea-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="783ea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="783ea-107">Prerequisites</span></span>
<span data-ttu-id="783ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="783ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="783ea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="783ea-110">Permission type</span></span>|<span data-ttu-id="783ea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="783ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="783ea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="783ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="783ea-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="783ea-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="783ea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="783ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="783ea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="783ea-115">Not supported.</span></span>|
|<span data-ttu-id="783ea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="783ea-116">Application</span></span>|<span data-ttu-id="783ea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="783ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="783ea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="783ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="783ea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="783ea-119">Request headers</span></span>
|<span data-ttu-id="783ea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="783ea-120">Header</span></span>|<span data-ttu-id="783ea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="783ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="783ea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="783ea-122">Authorization</span></span>|<span data-ttu-id="783ea-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="783ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="783ea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="783ea-124">Accept</span></span>|<span data-ttu-id="783ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="783ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="783ea-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="783ea-126">Request body</span></span>
<span data-ttu-id="783ea-127">В тексте запроса добавьте представление объекта Импортедвиндовсаутопилотдевицеидентитюплоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="783ea-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="783ea-128">В следующей таблице приведены свойства, необходимые при создании Импортедвиндовсаутопилотдевицеидентитюплоад.</span><span class="sxs-lookup"><span data-stu-id="783ea-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="783ea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="783ea-129">Property</span></span>|<span data-ttu-id="783ea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="783ea-130">Type</span></span>|<span data-ttu-id="783ea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="783ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="783ea-132">id</span><span class="sxs-lookup"><span data-stu-id="783ea-132">id</span></span>|<span data-ttu-id="783ea-133">String</span><span class="sxs-lookup"><span data-stu-id="783ea-133">String</span></span>|<span data-ttu-id="783ea-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="783ea-134">The GUID for the object</span></span>|
|<span data-ttu-id="783ea-135">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="783ea-135">createdDateTimeUtc</span></span>|<span data-ttu-id="783ea-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="783ea-136">DateTimeOffset</span></span>|<span data-ttu-id="783ea-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="783ea-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="783ea-138">status</span><span class="sxs-lookup"><span data-stu-id="783ea-138">status</span></span>|[<span data-ttu-id="783ea-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="783ea-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="783ea-140">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="783ea-140">Upload status.</span></span> <span data-ttu-id="783ea-141">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="783ea-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="783ea-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="783ea-142">Response</span></span>
<span data-ttu-id="783ea-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="783ea-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="783ea-144">Пример</span><span class="sxs-lookup"><span data-stu-id="783ea-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="783ea-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="783ea-145">Request</span></span>
<span data-ttu-id="783ea-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="783ea-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="783ea-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="783ea-147">Response</span></span>
<span data-ttu-id="783ea-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="783ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





