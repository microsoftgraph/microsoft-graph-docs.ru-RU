---
title: Обновление appLogCollectionRequest
description: Обновление свойств объекта appLogCollectionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83a03f5cc8d112ccbeaae83f4be808c84d91ccc6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945251"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="4be76-103">Обновление appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="4be76-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="4be76-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4be76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4be76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4be76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4be76-106">Обновление свойств объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4be76-106">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4be76-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4be76-107">Prerequisites</span></span>
<span data-ttu-id="4be76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4be76-110">Permission type</span></span>|<span data-ttu-id="4be76-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4be76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4be76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4be76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4be76-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be76-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4be76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4be76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4be76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4be76-115">Not supported.</span></span>|
|<span data-ttu-id="4be76-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4be76-116">Application</span></span>|<span data-ttu-id="4be76-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be76-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4be76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4be76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="4be76-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4be76-119">Request headers</span></span>
|<span data-ttu-id="4be76-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4be76-120">Header</span></span>|<span data-ttu-id="4be76-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4be76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4be76-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4be76-122">Authorization</span></span>|<span data-ttu-id="4be76-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4be76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4be76-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4be76-124">Accept</span></span>|<span data-ttu-id="4be76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4be76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4be76-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4be76-126">Request body</span></span>
<span data-ttu-id="4be76-127">В тексте запроса добавьте представление объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4be76-127">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="4be76-128">В следующей таблице приведены свойства, необходимые при создании [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="4be76-128">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="4be76-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4be76-129">Property</span></span>|<span data-ttu-id="4be76-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4be76-130">Type</span></span>|<span data-ttu-id="4be76-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4be76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4be76-132">id</span><span class="sxs-lookup"><span data-stu-id="4be76-132">id</span></span>|<span data-ttu-id="4be76-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4be76-133">String</span></span>|<span data-ttu-id="4be76-134">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4be76-134">The unique Identifier.</span></span> <span data-ttu-id="4be76-135">Это userId_DeviceId_AppId идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4be76-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="4be76-136">status</span><span class="sxs-lookup"><span data-stu-id="4be76-136">status</span></span>|[<span data-ttu-id="4be76-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="4be76-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="4be76-138">Запись состояния отправки.</span><span class="sxs-lookup"><span data-stu-id="4be76-138">Log upload status.</span></span> <span data-ttu-id="4be76-139">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4be76-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="4be76-140">Ошибк</span><span class="sxs-lookup"><span data-stu-id="4be76-140">errorMessage</span></span>|<span data-ttu-id="4be76-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4be76-141">String</span></span>|<span data-ttu-id="4be76-142">Сообщение об ошибке, если оно возникло во время процесса отправки</span><span class="sxs-lookup"><span data-stu-id="4be76-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="4be76-143">кустомлогфолдерс</span><span class="sxs-lookup"><span data-stu-id="4be76-143">customLogFolders</span></span>|<span data-ttu-id="4be76-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4be76-144">String collection</span></span>|<span data-ttu-id="4be76-145">Список папок журналов.</span><span class="sxs-lookup"><span data-stu-id="4be76-145">List of log folders.</span></span> |
|<span data-ttu-id="4be76-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4be76-146">completedDateTime</span></span>|<span data-ttu-id="4be76-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4be76-147">DateTimeOffset</span></span>|<span data-ttu-id="4be76-148">Время, когда запрос на отправку журнала достигает состояния терминала</span><span class="sxs-lookup"><span data-stu-id="4be76-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="4be76-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="4be76-149">Response</span></span>
<span data-ttu-id="4be76-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4be76-150">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be76-151">Пример</span><span class="sxs-lookup"><span data-stu-id="4be76-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="4be76-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="4be76-152">Request</span></span>
<span data-ttu-id="4be76-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4be76-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4be76-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4be76-154">Response</span></span>
<span data-ttu-id="4be76-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4be76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```





