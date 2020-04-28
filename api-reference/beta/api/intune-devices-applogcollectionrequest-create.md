---
title: Создание appLogCollectionRequest
description: Создание нового объекта appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fda135fbd3acb66e37da9cf33eb469f92b07e24f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426948"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="e229b-103">Создание appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e229b-103">Create appLogCollectionRequest</span></span>

<span data-ttu-id="e229b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e229b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e229b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e229b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e229b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e229b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e229b-107">Создание нового объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e229b-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e229b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e229b-108">Prerequisites</span></span>
<span data-ttu-id="e229b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e229b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e229b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e229b-111">Permission type</span></span>|<span data-ttu-id="e229b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e229b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e229b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e229b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e229b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e229b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e229b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e229b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e229b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e229b-116">Not supported.</span></span>|
|<span data-ttu-id="e229b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e229b-117">Application</span></span>|<span data-ttu-id="e229b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e229b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e229b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e229b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="e229b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e229b-120">Request headers</span></span>
|<span data-ttu-id="e229b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e229b-121">Header</span></span>|<span data-ttu-id="e229b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e229b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e229b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e229b-123">Authorization</span></span>|<span data-ttu-id="e229b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e229b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e229b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e229b-125">Accept</span></span>|<span data-ttu-id="e229b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e229b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e229b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e229b-127">Request body</span></span>
<span data-ttu-id="e229b-128">В тексте запроса добавьте представление объекта appLogCollectionRequest в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e229b-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="e229b-129">В следующей таблице приведены свойства, необходимые при создании appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="e229b-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="e229b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e229b-130">Property</span></span>|<span data-ttu-id="e229b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e229b-131">Type</span></span>|<span data-ttu-id="e229b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e229b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e229b-133">id</span><span class="sxs-lookup"><span data-stu-id="e229b-133">id</span></span>|<span data-ttu-id="e229b-134">String</span><span class="sxs-lookup"><span data-stu-id="e229b-134">String</span></span>|<span data-ttu-id="e229b-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e229b-135">The unique Identifier.</span></span> <span data-ttu-id="e229b-136">Это userId_DeviceId_AppId идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e229b-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="e229b-137">status</span><span class="sxs-lookup"><span data-stu-id="e229b-137">status</span></span>|[<span data-ttu-id="e229b-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="e229b-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="e229b-139">Запись состояния отправки.</span><span class="sxs-lookup"><span data-stu-id="e229b-139">Log upload status.</span></span> <span data-ttu-id="e229b-140">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e229b-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="e229b-141">Ошибк</span><span class="sxs-lookup"><span data-stu-id="e229b-141">errorMessage</span></span>|<span data-ttu-id="e229b-142">String</span><span class="sxs-lookup"><span data-stu-id="e229b-142">String</span></span>|<span data-ttu-id="e229b-143">Сообщение об ошибке, если оно возникло во время процесса отправки</span><span class="sxs-lookup"><span data-stu-id="e229b-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="e229b-144">кустомлогфолдерс</span><span class="sxs-lookup"><span data-stu-id="e229b-144">customLogFolders</span></span>|<span data-ttu-id="e229b-145">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e229b-145">String collection</span></span>|<span data-ttu-id="e229b-146">Список папок журналов.</span><span class="sxs-lookup"><span data-stu-id="e229b-146">List of log folders.</span></span> |
|<span data-ttu-id="e229b-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e229b-147">completedDateTime</span></span>|<span data-ttu-id="e229b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e229b-148">DateTimeOffset</span></span>|<span data-ttu-id="e229b-149">Время, когда запрос на отправку журнала достигает состояния терминала</span><span class="sxs-lookup"><span data-stu-id="e229b-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="e229b-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="e229b-150">Response</span></span>
<span data-ttu-id="e229b-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e229b-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e229b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e229b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e229b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e229b-153">Request</span></span>
<span data-ttu-id="e229b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e229b-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
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

### <a name="response"></a><span data-ttu-id="e229b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="e229b-155">Response</span></span>
<span data-ttu-id="e229b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e229b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



