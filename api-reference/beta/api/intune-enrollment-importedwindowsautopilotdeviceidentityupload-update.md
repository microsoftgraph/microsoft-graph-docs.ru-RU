---
title: Обновление Импортедвиндовсаутопилотдевицеидентитюплоад
description: Обновление свойств объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa2c38224d57dc7750b95b2a339ba0bb10b29f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145586"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="ed5a5-103">Обновление Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="ed5a5-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="ed5a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed5a5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed5a5-106">Обновление свойств объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="ed5a5-106">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed5a5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed5a5-107">Prerequisites</span></span>
<span data-ttu-id="ed5a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed5a5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed5a5-110">Permission type</span></span>|<span data-ttu-id="ed5a5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed5a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed5a5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed5a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed5a5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed5a5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed5a5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed5a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed5a5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-115">Not supported.</span></span>|
|<span data-ttu-id="ed5a5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed5a5-116">Application</span></span>|<span data-ttu-id="ed5a5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed5a5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed5a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="ed5a5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed5a5-119">Request headers</span></span>
|<span data-ttu-id="ed5a5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed5a5-120">Header</span></span>|<span data-ttu-id="ed5a5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ed5a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed5a5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed5a5-122">Authorization</span></span>|<span data-ttu-id="ed5a5-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed5a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed5a5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ed5a5-124">Accept</span></span>|<span data-ttu-id="ed5a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed5a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed5a5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed5a5-126">Request body</span></span>
<span data-ttu-id="ed5a5-127">В тексте запроса добавьте представление объекта [Импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="ed5a5-128">В следующей таблице приведены свойства, необходимые при создании [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="ed5a5-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="ed5a5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed5a5-129">Property</span></span>|<span data-ttu-id="ed5a5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ed5a5-130">Type</span></span>|<span data-ttu-id="ed5a5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ed5a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed5a5-132">id</span><span class="sxs-lookup"><span data-stu-id="ed5a5-132">id</span></span>|<span data-ttu-id="ed5a5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ed5a5-133">String</span></span>|<span data-ttu-id="ed5a5-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="ed5a5-134">The GUID for the object</span></span>|
|<span data-ttu-id="ed5a5-135">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="ed5a5-135">createdDateTimeUtc</span></span>|<span data-ttu-id="ed5a5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed5a5-136">DateTimeOffset</span></span>|<span data-ttu-id="ed5a5-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="ed5a5-138">status</span><span class="sxs-lookup"><span data-stu-id="ed5a5-138">status</span></span>|[<span data-ttu-id="ed5a5-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="ed5a5-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="ed5a5-140">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-140">Upload status.</span></span> <span data-ttu-id="ed5a5-141">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="ed5a5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed5a5-142">Response</span></span>
<span data-ttu-id="ed5a5-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-143">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed5a5-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ed5a5-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed5a5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed5a5-145">Request</span></span>
<span data-ttu-id="ed5a5-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed5a5-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed5a5-147">Response</span></span>
<span data-ttu-id="ed5a5-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed5a5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




