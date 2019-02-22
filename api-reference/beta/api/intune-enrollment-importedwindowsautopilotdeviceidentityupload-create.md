---
title: Создание Импортедвиндовсаутопилотдевицеидентитюплоад
description: Создание нового объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 124b54760c6fc77668c16562a865912257a3e8e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169904"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="c2ff4-103">Создание Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="c2ff4-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="c2ff4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2ff4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2ff4-106">Создание нового объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="c2ff4-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2ff4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2ff4-107">Prerequisites</span></span>
<span data-ttu-id="c2ff4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2ff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c2ff4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ff4-110">Permission type</span></span>|<span data-ttu-id="c2ff4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2ff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2ff4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2ff4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2ff4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ff4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c2ff4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2ff4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2ff4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-115">Not supported.</span></span>|
|<span data-ttu-id="c2ff4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2ff4-116">Application</span></span>|<span data-ttu-id="c2ff4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2ff4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2ff4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="c2ff4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2ff4-119">Request headers</span></span>
|<span data-ttu-id="c2ff4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2ff4-120">Header</span></span>|<span data-ttu-id="c2ff4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c2ff4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2ff4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2ff4-122">Authorization</span></span>|<span data-ttu-id="c2ff4-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2ff4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2ff4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c2ff4-124">Accept</span></span>|<span data-ttu-id="c2ff4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2ff4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2ff4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2ff4-126">Request body</span></span>
<span data-ttu-id="c2ff4-127">В тексте запроса добавьте представление объекта Импортедвиндовсаутопилотдевицеидентитюплоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="c2ff4-128">В следующей таблице приведены свойства, необходимые при создании Импортедвиндовсаутопилотдевицеидентитюплоад.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="c2ff4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2ff4-129">Property</span></span>|<span data-ttu-id="c2ff4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c2ff4-130">Type</span></span>|<span data-ttu-id="c2ff4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ff4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2ff4-132">id</span><span class="sxs-lookup"><span data-stu-id="c2ff4-132">id</span></span>|<span data-ttu-id="c2ff4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c2ff4-133">String</span></span>|<span data-ttu-id="c2ff4-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="c2ff4-134">The GUID for the object</span></span>|
|<span data-ttu-id="c2ff4-135">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="c2ff4-135">createdDateTimeUtc</span></span>|<span data-ttu-id="c2ff4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2ff4-136">DateTimeOffset</span></span>|<span data-ttu-id="c2ff4-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="c2ff4-138">status</span><span class="sxs-lookup"><span data-stu-id="c2ff4-138">status</span></span>|[<span data-ttu-id="c2ff4-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="c2ff4-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="c2ff4-140">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-140">Upload status.</span></span> <span data-ttu-id="c2ff4-141">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="c2ff4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ff4-142">Response</span></span>
<span data-ttu-id="c2ff4-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ff4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c2ff4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2ff4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2ff4-145">Request</span></span>
<span data-ttu-id="c2ff4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2ff4-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2ff4-147">Response</span></span>
<span data-ttu-id="c2ff4-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2ff4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




