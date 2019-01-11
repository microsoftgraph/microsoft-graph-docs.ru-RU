---
title: Обновление importedWindowsAutopilotDeviceIdentityUpload
description: Обновление свойства объекта importedWindowsAutopilotDeviceIdentityUpload.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76e699ebf7f0704ab6a524c1c5869339e0318ec2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894378"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="252f5-103">Обновление importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="252f5-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="252f5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="252f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="252f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="252f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="252f5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="252f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="252f5-107">Обновление свойства объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="252f5-107">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="252f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="252f5-108">Prerequisites</span></span>
<span data-ttu-id="252f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="252f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="252f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="252f5-111">Permission type</span></span>|<span data-ttu-id="252f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="252f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="252f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="252f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="252f5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="252f5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="252f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="252f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="252f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="252f5-116">Not supported.</span></span>|
|<span data-ttu-id="252f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="252f5-117">Application</span></span>|<span data-ttu-id="252f5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="252f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="252f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="252f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="252f5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="252f5-120">Request headers</span></span>
|<span data-ttu-id="252f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="252f5-121">Header</span></span>|<span data-ttu-id="252f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="252f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="252f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="252f5-123">Authorization</span></span>|<span data-ttu-id="252f5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="252f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="252f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="252f5-125">Accept</span></span>|<span data-ttu-id="252f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="252f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="252f5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="252f5-127">Request body</span></span>
<span data-ttu-id="252f5-128">В тексте запроса укажите представление JSON для объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="252f5-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="252f5-129">В следующей таблице показаны свойства, которые необходимы для создания [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="252f5-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="252f5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="252f5-130">Property</span></span>|<span data-ttu-id="252f5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="252f5-131">Type</span></span>|<span data-ttu-id="252f5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="252f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252f5-133">id</span><span class="sxs-lookup"><span data-stu-id="252f5-133">id</span></span>|<span data-ttu-id="252f5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="252f5-134">String</span></span>|<span data-ttu-id="252f5-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="252f5-135">The GUID for the object</span></span>|
|<span data-ttu-id="252f5-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="252f5-136">createdDateTimeUtc</span></span>|<span data-ttu-id="252f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="252f5-137">DateTimeOffset</span></span>|<span data-ttu-id="252f5-138">Дата и время при создании сущности.</span><span class="sxs-lookup"><span data-stu-id="252f5-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="252f5-139">status</span><span class="sxs-lookup"><span data-stu-id="252f5-139">status</span></span>|[<span data-ttu-id="252f5-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="252f5-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="252f5-141">Отправьте состояние.</span><span class="sxs-lookup"><span data-stu-id="252f5-141">Upload status.</span></span> <span data-ttu-id="252f5-142">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="252f5-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="252f5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="252f5-143">Response</span></span>
<span data-ttu-id="252f5-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="252f5-144">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="252f5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="252f5-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="252f5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="252f5-146">Request</span></span>
<span data-ttu-id="252f5-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="252f5-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="252f5-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="252f5-148">Response</span></span>
<span data-ttu-id="252f5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="252f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





