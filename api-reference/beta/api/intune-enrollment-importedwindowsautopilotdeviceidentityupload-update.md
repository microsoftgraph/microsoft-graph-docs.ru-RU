---
title: Обновление importedWindowsAutopilotDeviceIdentityUpload
description: Обновление свойства объекта importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cca9472b0ceee0daa4bff04543141a7afe66eb78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949999"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="0126d-103">Обновление importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="0126d-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="0126d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0126d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0126d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0126d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0126d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0126d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0126d-107">Обновление свойства объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="0126d-107">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0126d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0126d-108">Prerequisites</span></span>
<span data-ttu-id="0126d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0126d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0126d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0126d-111">Permission type</span></span>|<span data-ttu-id="0126d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0126d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0126d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0126d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0126d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0126d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0126d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0126d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0126d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0126d-116">Not supported.</span></span>|
|<span data-ttu-id="0126d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0126d-117">Application</span></span>|<span data-ttu-id="0126d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0126d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0126d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0126d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="0126d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0126d-120">Request headers</span></span>
|<span data-ttu-id="0126d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0126d-121">Header</span></span>|<span data-ttu-id="0126d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0126d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0126d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0126d-123">Authorization</span></span>|<span data-ttu-id="0126d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0126d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0126d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0126d-125">Accept</span></span>|<span data-ttu-id="0126d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0126d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0126d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0126d-127">Request body</span></span>
<span data-ttu-id="0126d-128">В тексте запроса укажите представление JSON для объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="0126d-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="0126d-129">В следующей таблице показаны свойства, которые необходимы для создания [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="0126d-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="0126d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0126d-130">Property</span></span>|<span data-ttu-id="0126d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0126d-131">Type</span></span>|<span data-ttu-id="0126d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0126d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0126d-133">id</span><span class="sxs-lookup"><span data-stu-id="0126d-133">id</span></span>|<span data-ttu-id="0126d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0126d-134">String</span></span>|<span data-ttu-id="0126d-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="0126d-135">The GUID for the object</span></span>|
|<span data-ttu-id="0126d-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="0126d-136">createdDateTimeUtc</span></span>|<span data-ttu-id="0126d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0126d-137">DateTimeOffset</span></span>|<span data-ttu-id="0126d-138">Дата и время при создании сущности.</span><span class="sxs-lookup"><span data-stu-id="0126d-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="0126d-139">status</span><span class="sxs-lookup"><span data-stu-id="0126d-139">status</span></span>|[<span data-ttu-id="0126d-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="0126d-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="0126d-141">Отправьте состояние.</span><span class="sxs-lookup"><span data-stu-id="0126d-141">Upload status.</span></span> <span data-ttu-id="0126d-142">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="0126d-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="0126d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0126d-143">Response</span></span>
<span data-ttu-id="0126d-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0126d-144">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0126d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="0126d-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="0126d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="0126d-146">Request</span></span>
<span data-ttu-id="0126d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0126d-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="0126d-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="0126d-148">Response</span></span>
<span data-ttu-id="0126d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0126d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





