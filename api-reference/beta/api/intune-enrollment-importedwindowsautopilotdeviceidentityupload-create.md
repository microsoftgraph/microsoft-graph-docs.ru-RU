---
title: Создание importedWindowsAutopilotDeviceIdentityUpload
description: Создание нового объекта importedWindowsAutopilotDeviceIdentityUpload.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e47e3c8545335f0f34511e7d0b87bf2bd54d2162
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396814"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="dce9a-103">Создание importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="dce9a-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="dce9a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dce9a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dce9a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dce9a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dce9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce9a-107">Создание нового объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="dce9a-107">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dce9a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="dce9a-108">Prerequisites</span></span>
<span data-ttu-id="dce9a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dce9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dce9a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dce9a-111">Permission type</span></span>|<span data-ttu-id="dce9a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dce9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dce9a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dce9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dce9a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dce9a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dce9a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dce9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dce9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce9a-116">Not supported.</span></span>|
|<span data-ttu-id="dce9a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dce9a-117">Application</span></span>|<span data-ttu-id="dce9a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dce9a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dce9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="dce9a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dce9a-120">Request headers</span></span>
|<span data-ttu-id="dce9a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dce9a-121">Header</span></span>|<span data-ttu-id="dce9a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dce9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dce9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dce9a-123">Authorization</span></span>|<span data-ttu-id="dce9a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dce9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dce9a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dce9a-125">Accept</span></span>|<span data-ttu-id="dce9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dce9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dce9a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dce9a-127">Request body</span></span>
<span data-ttu-id="dce9a-128">В тексте запроса укажите представление JSON для объекта importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="dce9a-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="dce9a-129">В следующей таблице показаны свойства, которые необходимы для создания importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="dce9a-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="dce9a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dce9a-130">Property</span></span>|<span data-ttu-id="dce9a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dce9a-131">Type</span></span>|<span data-ttu-id="dce9a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dce9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dce9a-133">id</span><span class="sxs-lookup"><span data-stu-id="dce9a-133">id</span></span>|<span data-ttu-id="dce9a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dce9a-134">String</span></span>|<span data-ttu-id="dce9a-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="dce9a-135">The GUID for the object</span></span>|
|<span data-ttu-id="dce9a-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="dce9a-136">createdDateTimeUtc</span></span>|<span data-ttu-id="dce9a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dce9a-137">DateTimeOffset</span></span>|<span data-ttu-id="dce9a-138">Дата и время при создании сущности.</span><span class="sxs-lookup"><span data-stu-id="dce9a-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="dce9a-139">status</span><span class="sxs-lookup"><span data-stu-id="dce9a-139">status</span></span>|[<span data-ttu-id="dce9a-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="dce9a-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="dce9a-141">Отправьте состояние.</span><span class="sxs-lookup"><span data-stu-id="dce9a-141">Upload status.</span></span> <span data-ttu-id="dce9a-142">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="dce9a-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="dce9a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dce9a-143">Response</span></span>
<span data-ttu-id="dce9a-144">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dce9a-144">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce9a-145">Пример</span><span class="sxs-lookup"><span data-stu-id="dce9a-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="dce9a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="dce9a-146">Request</span></span>
<span data-ttu-id="dce9a-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dce9a-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dce9a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="dce9a-148">Response</span></span>
<span data-ttu-id="dce9a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dce9a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




