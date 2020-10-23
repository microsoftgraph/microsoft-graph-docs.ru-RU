---
title: Обновление appLogCollectionRequest
description: Обновление свойств объекта appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0f77bdc0a5f8b87d28eac3a1e2fd542c5c9a48b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735521"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="48f03-103">Обновление appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="48f03-103">Update appLogCollectionRequest</span></span>

<span data-ttu-id="48f03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48f03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48f03-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48f03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48f03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48f03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48f03-107">Обновление свойств объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="48f03-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48f03-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48f03-108">Prerequisites</span></span>
<span data-ttu-id="48f03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48f03-111">Permission type</span></span>|<span data-ttu-id="48f03-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48f03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48f03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48f03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48f03-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f03-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="48f03-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48f03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48f03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48f03-116">Not supported.</span></span>|
|<span data-ttu-id="48f03-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48f03-117">Application</span></span>|<span data-ttu-id="48f03-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f03-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48f03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48f03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="48f03-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="48f03-120">Request headers</span></span>
|<span data-ttu-id="48f03-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48f03-121">Header</span></span>|<span data-ttu-id="48f03-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48f03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48f03-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48f03-123">Authorization</span></span>|<span data-ttu-id="48f03-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48f03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48f03-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48f03-125">Accept</span></span>|<span data-ttu-id="48f03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48f03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48f03-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48f03-127">Request body</span></span>
<span data-ttu-id="48f03-128">В тексте запроса добавьте представление объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48f03-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="48f03-129">В следующей таблице приведены свойства, необходимые при создании [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span><span class="sxs-lookup"><span data-stu-id="48f03-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="48f03-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48f03-130">Property</span></span>|<span data-ttu-id="48f03-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48f03-131">Type</span></span>|<span data-ttu-id="48f03-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48f03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48f03-133">id</span><span class="sxs-lookup"><span data-stu-id="48f03-133">id</span></span>|<span data-ttu-id="48f03-134">Строка</span><span class="sxs-lookup"><span data-stu-id="48f03-134">String</span></span>|<span data-ttu-id="48f03-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="48f03-135">The unique Identifier.</span></span> <span data-ttu-id="48f03-136">Это userId_DeviceId_AppId идентификатор.</span><span class="sxs-lookup"><span data-stu-id="48f03-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="48f03-137">status</span><span class="sxs-lookup"><span data-stu-id="48f03-137">status</span></span>|[<span data-ttu-id="48f03-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="48f03-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="48f03-139">Запись состояния отправки.</span><span class="sxs-lookup"><span data-stu-id="48f03-139">Log upload status.</span></span> <span data-ttu-id="48f03-140">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="48f03-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="48f03-141">Ошибк</span><span class="sxs-lookup"><span data-stu-id="48f03-141">errorMessage</span></span>|<span data-ttu-id="48f03-142">Строка</span><span class="sxs-lookup"><span data-stu-id="48f03-142">String</span></span>|<span data-ttu-id="48f03-143">Сообщение об ошибке, если оно возникло во время процесса отправки</span><span class="sxs-lookup"><span data-stu-id="48f03-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="48f03-144">кустомлогфолдерс</span><span class="sxs-lookup"><span data-stu-id="48f03-144">customLogFolders</span></span>|<span data-ttu-id="48f03-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="48f03-145">String collection</span></span>|<span data-ttu-id="48f03-146">Список папок журналов.</span><span class="sxs-lookup"><span data-stu-id="48f03-146">List of log folders.</span></span> |
|<span data-ttu-id="48f03-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="48f03-147">completedDateTime</span></span>|<span data-ttu-id="48f03-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48f03-148">DateTimeOffset</span></span>|<span data-ttu-id="48f03-149">Время, когда запрос на отправку журнала достигает состояния терминала</span><span class="sxs-lookup"><span data-stu-id="48f03-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="48f03-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="48f03-150">Response</span></span>
<span data-ttu-id="48f03-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48f03-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48f03-152">Пример</span><span class="sxs-lookup"><span data-stu-id="48f03-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="48f03-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="48f03-153">Request</span></span>
<span data-ttu-id="48f03-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48f03-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48f03-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="48f03-155">Response</span></span>
<span data-ttu-id="48f03-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48f03-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





