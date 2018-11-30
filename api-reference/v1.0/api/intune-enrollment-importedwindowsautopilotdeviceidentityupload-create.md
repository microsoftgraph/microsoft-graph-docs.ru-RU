---
title: Создание importedWindowsAutopilotDeviceIdentityUpload
description: Создание нового объекта importedWindowsAutopilotDeviceIdentityUpload.
ms.openlocfilehash: ff5c28e115499a0b22d977c0d2b6ece1c0d99ad0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026602"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="f6bad-103">Создание importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="f6bad-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="f6bad-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f6bad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6bad-105">Создание нового объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="f6bad-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6bad-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6bad-106">Prerequisites</span></span>
<span data-ttu-id="f6bad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6bad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6bad-109">Permission type</span></span>|<span data-ttu-id="f6bad-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6bad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6bad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6bad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6bad-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bad-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6bad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6bad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6bad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6bad-114">Not supported.</span></span>|
|<span data-ttu-id="f6bad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6bad-115">Application</span></span>|<span data-ttu-id="f6bad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6bad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6bad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6bad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="f6bad-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6bad-118">Request headers</span></span>
|<span data-ttu-id="f6bad-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6bad-119">Header</span></span>|<span data-ttu-id="f6bad-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f6bad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6bad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6bad-121">Authorization</span></span>|<span data-ttu-id="f6bad-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f6bad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6bad-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f6bad-123">Accept</span></span>|<span data-ttu-id="f6bad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f6bad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6bad-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6bad-125">Request body</span></span>
<span data-ttu-id="f6bad-126">В тексте запроса укажите представление JSON для объекта importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="f6bad-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="f6bad-127">В следующей таблице показаны свойства, которые необходимы для создания importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="f6bad-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="f6bad-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6bad-128">Property</span></span>|<span data-ttu-id="f6bad-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f6bad-129">Type</span></span>|<span data-ttu-id="f6bad-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f6bad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6bad-131">id</span><span class="sxs-lookup"><span data-stu-id="f6bad-131">id</span></span>|<span data-ttu-id="f6bad-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f6bad-132">String</span></span>|<span data-ttu-id="f6bad-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="f6bad-133">The GUID for the object</span></span>|
|<span data-ttu-id="f6bad-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="f6bad-134">createdDateTimeUtc</span></span>|<span data-ttu-id="f6bad-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6bad-135">DateTimeOffset</span></span>|<span data-ttu-id="f6bad-136">Дата и время при создании сущности.</span><span class="sxs-lookup"><span data-stu-id="f6bad-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="f6bad-137">status</span><span class="sxs-lookup"><span data-stu-id="f6bad-137">status</span></span>|[<span data-ttu-id="f6bad-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="f6bad-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="f6bad-139">Отправьте состояние.</span><span class="sxs-lookup"><span data-stu-id="f6bad-139">Upload status.</span></span> <span data-ttu-id="f6bad-140">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="f6bad-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="f6bad-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6bad-141">Response</span></span>
<span data-ttu-id="f6bad-142">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f6bad-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6bad-143">Пример</span><span class="sxs-lookup"><span data-stu-id="f6bad-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6bad-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6bad-144">Request</span></span>
<span data-ttu-id="f6bad-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6bad-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6bad-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6bad-146">Response</span></span>
<span data-ttu-id="f6bad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f6bad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



