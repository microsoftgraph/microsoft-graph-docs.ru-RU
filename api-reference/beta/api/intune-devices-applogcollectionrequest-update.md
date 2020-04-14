---
title: Обновление appLogCollectionRequest
description: Обновление свойств объекта appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6592e8a1d0eb27afff70b1d49ab7a1cfe108e4a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381075"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="3a3bb-103">Обновление appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="3a3bb-103">Update appLogCollectionRequest</span></span>

<span data-ttu-id="3a3bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a3bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a3bb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a3bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a3bb-107">Обновление свойств объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3a3bb-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a3bb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a3bb-108">Prerequisites</span></span>
<span data-ttu-id="3a3bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a3bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a3bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3bb-111">Permission type</span></span>|<span data-ttu-id="3a3bb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a3bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a3bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a3bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a3bb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a3bb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3a3bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a3bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a3bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-116">Not supported.</span></span>|
|<span data-ttu-id="3a3bb-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3a3bb-117">Application</span></span>|<span data-ttu-id="3a3bb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a3bb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a3bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a3bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="3a3bb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a3bb-120">Request headers</span></span>
|<span data-ttu-id="3a3bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a3bb-121">Header</span></span>|<span data-ttu-id="3a3bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a3bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a3bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a3bb-123">Authorization</span></span>|<span data-ttu-id="3a3bb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a3bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a3bb-125">Accept</span></span>|<span data-ttu-id="3a3bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a3bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a3bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a3bb-127">Request body</span></span>
<span data-ttu-id="3a3bb-128">В тексте запроса добавьте представление объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="3a3bb-129">В следующей таблице приведены свойства, необходимые при создании [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="3a3bb-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="3a3bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a3bb-130">Property</span></span>|<span data-ttu-id="3a3bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a3bb-131">Type</span></span>|<span data-ttu-id="3a3bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a3bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a3bb-133">id</span><span class="sxs-lookup"><span data-stu-id="3a3bb-133">id</span></span>|<span data-ttu-id="3a3bb-134">String</span><span class="sxs-lookup"><span data-stu-id="3a3bb-134">String</span></span>|<span data-ttu-id="3a3bb-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-135">The unique Identifier.</span></span> <span data-ttu-id="3a3bb-136">Это userId_DeviceId_AppId идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="3a3bb-137">status</span><span class="sxs-lookup"><span data-stu-id="3a3bb-137">status</span></span>|[<span data-ttu-id="3a3bb-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="3a3bb-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="3a3bb-139">Запись состояния отправки.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-139">Log upload status.</span></span> <span data-ttu-id="3a3bb-140">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="3a3bb-141">Ошибк</span><span class="sxs-lookup"><span data-stu-id="3a3bb-141">errorMessage</span></span>|<span data-ttu-id="3a3bb-142">String</span><span class="sxs-lookup"><span data-stu-id="3a3bb-142">String</span></span>|<span data-ttu-id="3a3bb-143">Сообщение об ошибке, если оно возникло во время процесса отправки</span><span class="sxs-lookup"><span data-stu-id="3a3bb-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="3a3bb-144">кустомлогфолдерс</span><span class="sxs-lookup"><span data-stu-id="3a3bb-144">customLogFolders</span></span>|<span data-ttu-id="3a3bb-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a3bb-145">String collection</span></span>|<span data-ttu-id="3a3bb-146">Список папок журналов.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-146">List of log folders.</span></span> |
|<span data-ttu-id="3a3bb-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a3bb-147">completedDateTime</span></span>|<span data-ttu-id="3a3bb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a3bb-148">DateTimeOffset</span></span>|<span data-ttu-id="3a3bb-149">Время, когда запрос на отправку журнала достигает состояния терминала</span><span class="sxs-lookup"><span data-stu-id="3a3bb-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="3a3bb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a3bb-150">Response</span></span>
<span data-ttu-id="3a3bb-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3bb-152">Пример</span><span class="sxs-lookup"><span data-stu-id="3a3bb-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a3bb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a3bb-153">Request</span></span>
<span data-ttu-id="3a3bb-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a3bb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a3bb-155">Response</span></span>
<span data-ttu-id="3a3bb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a3bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



