---
title: Создание appLogCollectionRequest
description: Создайте новый объект appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbd19f042c6dbfe80a4c02ec224fde5b1e5fb696
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136484"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="20475-103">Создание appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="20475-103">Create appLogCollectionRequest</span></span>

<span data-ttu-id="20475-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20475-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20475-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20475-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20475-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20475-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20475-107">Создайте новый [объект appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="20475-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20475-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20475-108">Prerequisites</span></span>
<span data-ttu-id="20475-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20475-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20475-111">Permission type</span></span>|<span data-ttu-id="20475-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20475-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20475-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20475-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20475-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20475-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20475-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20475-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20475-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20475-116">Not supported.</span></span>|
|<span data-ttu-id="20475-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="20475-117">Application</span></span>|<span data-ttu-id="20475-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20475-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20475-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20475-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="20475-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="20475-120">Request headers</span></span>
|<span data-ttu-id="20475-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20475-121">Header</span></span>|<span data-ttu-id="20475-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20475-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20475-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20475-123">Authorization</span></span>|<span data-ttu-id="20475-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20475-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20475-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20475-125">Accept</span></span>|<span data-ttu-id="20475-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20475-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20475-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20475-127">Request body</span></span>
<span data-ttu-id="20475-128">В теле запроса поставляем представление JSON для объекта appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="20475-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="20475-129">В следующей таблице показаны свойства, необходимые при создании appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="20475-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="20475-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20475-130">Property</span></span>|<span data-ttu-id="20475-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20475-131">Type</span></span>|<span data-ttu-id="20475-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20475-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20475-133">id</span><span class="sxs-lookup"><span data-stu-id="20475-133">id</span></span>|<span data-ttu-id="20475-134">Строка</span><span class="sxs-lookup"><span data-stu-id="20475-134">String</span></span>|<span data-ttu-id="20475-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="20475-135">The unique Identifier.</span></span> <span data-ttu-id="20475-136">Это userId_DeviceId_AppId id.</span><span class="sxs-lookup"><span data-stu-id="20475-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="20475-137">status</span><span class="sxs-lookup"><span data-stu-id="20475-137">status</span></span>|[<span data-ttu-id="20475-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="20475-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="20475-139">Состояние загрузки журнала.</span><span class="sxs-lookup"><span data-stu-id="20475-139">Log upload status.</span></span> <span data-ttu-id="20475-140">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="20475-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="20475-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="20475-141">errorMessage</span></span>|<span data-ttu-id="20475-142">Строка</span><span class="sxs-lookup"><span data-stu-id="20475-142">String</span></span>|<span data-ttu-id="20475-143">Сообщение об ошибке, если таково сообщение во время процесса загрузки</span><span class="sxs-lookup"><span data-stu-id="20475-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="20475-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="20475-144">customLogFolders</span></span>|<span data-ttu-id="20475-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="20475-145">String collection</span></span>|<span data-ttu-id="20475-146">Список папок журнала.</span><span class="sxs-lookup"><span data-stu-id="20475-146">List of log folders.</span></span> |
|<span data-ttu-id="20475-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="20475-147">completedDateTime</span></span>|<span data-ttu-id="20475-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20475-148">DateTimeOffset</span></span>|<span data-ttu-id="20475-149">Время, в течение которого запрос журнала загрузки достиг состояния терминала</span><span class="sxs-lookup"><span data-stu-id="20475-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="20475-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="20475-150">Response</span></span>
<span data-ttu-id="20475-151">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20475-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20475-152">Пример</span><span class="sxs-lookup"><span data-stu-id="20475-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="20475-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="20475-153">Request</span></span>
<span data-ttu-id="20475-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20475-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20475-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="20475-155">Response</span></span>
<span data-ttu-id="20475-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20475-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




