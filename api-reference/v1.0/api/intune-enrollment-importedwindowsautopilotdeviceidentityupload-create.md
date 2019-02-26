---
title: Создание Импортедвиндовсаутопилотдевицеидентитюплоад
description: Создание нового объекта Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fd4230b0ecdb4279380255b1fa62cbe697a4843
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264395"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="7cced-103">Создание Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="7cced-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="7cced-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7cced-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cced-105">Создание нового объекта [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="7cced-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cced-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7cced-106">Prerequisites</span></span>
<span data-ttu-id="7cced-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7cced-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cced-109">Permission type</span></span>|<span data-ttu-id="7cced-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cced-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cced-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cced-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7cced-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cced-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7cced-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cced-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cced-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cced-114">Not supported.</span></span>|
|<span data-ttu-id="7cced-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cced-115">Application</span></span>|<span data-ttu-id="7cced-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cced-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cced-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cced-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="7cced-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cced-118">Request headers</span></span>
|<span data-ttu-id="7cced-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cced-119">Header</span></span>|<span data-ttu-id="7cced-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7cced-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cced-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cced-121">Authorization</span></span>|<span data-ttu-id="7cced-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7cced-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cced-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7cced-123">Accept</span></span>|<span data-ttu-id="7cced-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7cced-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cced-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cced-125">Request body</span></span>
<span data-ttu-id="7cced-126">В тексте запроса добавьте представление объекта Импортедвиндовсаутопилотдевицеидентитюплоад в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cced-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="7cced-127">В следующей таблице приведены свойства, необходимые при создании Импортедвиндовсаутопилотдевицеидентитюплоад.</span><span class="sxs-lookup"><span data-stu-id="7cced-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="7cced-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cced-128">Property</span></span>|<span data-ttu-id="7cced-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7cced-129">Type</span></span>|<span data-ttu-id="7cced-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7cced-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cced-131">id</span><span class="sxs-lookup"><span data-stu-id="7cced-131">id</span></span>|<span data-ttu-id="7cced-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7cced-132">String</span></span>|<span data-ttu-id="7cced-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="7cced-133">The GUID for the object</span></span>|
|<span data-ttu-id="7cced-134">Креатеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="7cced-134">createdDateTimeUtc</span></span>|<span data-ttu-id="7cced-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cced-135">DateTimeOffset</span></span>|<span data-ttu-id="7cced-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7cced-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="7cced-137">status</span><span class="sxs-lookup"><span data-stu-id="7cced-137">status</span></span>|[<span data-ttu-id="7cced-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="7cced-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="7cced-139">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7cced-139">Upload status.</span></span> <span data-ttu-id="7cced-140">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="7cced-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="7cced-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cced-141">Response</span></span>
<span data-ttu-id="7cced-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7cced-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cced-143">Пример</span><span class="sxs-lookup"><span data-stu-id="7cced-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cced-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cced-144">Request</span></span>
<span data-ttu-id="7cced-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cced-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7cced-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cced-146">Response</span></span>
<span data-ttu-id="7cced-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7cced-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



