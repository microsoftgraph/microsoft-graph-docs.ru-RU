---
title: Создание Импортедвиндовсаутопилотдевицеидентитюплоад
description: Создание нового объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa2fd3cda5995b9e5a66754599393bd60ae0db7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561021"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="b1245-103">Создание Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="b1245-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="b1245-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1245-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1245-105">Создание нового объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="b1245-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1245-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1245-106">Prerequisites</span></span>
<span data-ttu-id="b1245-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1245-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1245-109">Permission type</span></span>|<span data-ttu-id="b1245-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1245-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1245-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1245-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1245-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1245-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1245-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1245-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1245-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1245-114">Not supported.</span></span>|
|<span data-ttu-id="b1245-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1245-115">Application</span></span>|<span data-ttu-id="b1245-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1245-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1245-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1245-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="b1245-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1245-118">Request headers</span></span>
|<span data-ttu-id="b1245-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1245-119">Header</span></span>|<span data-ttu-id="b1245-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b1245-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1245-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1245-121">Authorization</span></span>|<span data-ttu-id="b1245-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1245-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1245-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b1245-123">Accept</span></span>|<span data-ttu-id="b1245-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1245-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1245-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1245-125">Request body</span></span>
<span data-ttu-id="b1245-126">В тексте запроса добавьте представление объекта Импортедвиндовсаутопилотдевицеидентитюплоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1245-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="b1245-127">В следующей таблице приведены свойства, необходимые при создании Импортедвиндовсаутопилотдевицеидентитюплоад.</span><span class="sxs-lookup"><span data-stu-id="b1245-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="b1245-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1245-128">Property</span></span>|<span data-ttu-id="b1245-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b1245-129">Type</span></span>|<span data-ttu-id="b1245-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b1245-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1245-131">id</span><span class="sxs-lookup"><span data-stu-id="b1245-131">id</span></span>|<span data-ttu-id="b1245-132">String</span><span class="sxs-lookup"><span data-stu-id="b1245-132">String</span></span>|<span data-ttu-id="b1245-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b1245-133">The GUID for the object</span></span>|
|<span data-ttu-id="b1245-134">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="b1245-134">createdDateTimeUtc</span></span>|<span data-ttu-id="b1245-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1245-135">DateTimeOffset</span></span>|<span data-ttu-id="b1245-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b1245-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="b1245-137">status</span><span class="sxs-lookup"><span data-stu-id="b1245-137">status</span></span>|[<span data-ttu-id="b1245-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b1245-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="b1245-139">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b1245-139">Upload status.</span></span> <span data-ttu-id="b1245-140">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="b1245-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="b1245-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1245-141">Response</span></span>
<span data-ttu-id="b1245-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1245-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1245-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b1245-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1245-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1245-144">Request</span></span>
<span data-ttu-id="b1245-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1245-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1245-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1245-146">Response</span></span>
<span data-ttu-id="b1245-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1245-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



