---
title: Создание appLogCollectionRequest
description: Создание нового объекта appLogCollectionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83a4c20b64ff0d0a39b4bb736f8f89864df2f6e1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959336"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="1d25a-103">Создание appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="1d25a-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="1d25a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d25a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d25a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d25a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d25a-106">Создание нового объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="1d25a-106">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d25a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d25a-107">Prerequisites</span></span>
<span data-ttu-id="1d25a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d25a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d25a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d25a-110">Permission type</span></span>|<span data-ttu-id="1d25a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d25a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d25a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d25a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d25a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d25a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1d25a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d25a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d25a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d25a-115">Not supported.</span></span>|
|<span data-ttu-id="1d25a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d25a-116">Application</span></span>|<span data-ttu-id="1d25a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d25a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d25a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d25a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="1d25a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d25a-119">Request headers</span></span>
|<span data-ttu-id="1d25a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d25a-120">Header</span></span>|<span data-ttu-id="1d25a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1d25a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d25a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d25a-122">Authorization</span></span>|<span data-ttu-id="1d25a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d25a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d25a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1d25a-124">Accept</span></span>|<span data-ttu-id="1d25a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d25a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d25a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d25a-126">Request body</span></span>
<span data-ttu-id="1d25a-127">В тексте запроса добавьте представление объекта appLogCollectionRequest в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d25a-127">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="1d25a-128">В следующей таблице приведены свойства, необходимые при создании appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="1d25a-128">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="1d25a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d25a-129">Property</span></span>|<span data-ttu-id="1d25a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1d25a-130">Type</span></span>|<span data-ttu-id="1d25a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1d25a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d25a-132">id</span><span class="sxs-lookup"><span data-stu-id="1d25a-132">id</span></span>|<span data-ttu-id="1d25a-133">String</span><span class="sxs-lookup"><span data-stu-id="1d25a-133">String</span></span>|<span data-ttu-id="1d25a-134">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1d25a-134">The unique Identifier.</span></span> <span data-ttu-id="1d25a-135">Это идентификатор Усерид_девицеид_аппид.</span><span class="sxs-lookup"><span data-stu-id="1d25a-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="1d25a-136">status</span><span class="sxs-lookup"><span data-stu-id="1d25a-136">status</span></span>|[<span data-ttu-id="1d25a-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="1d25a-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="1d25a-138">Запись состояния отправки.</span><span class="sxs-lookup"><span data-stu-id="1d25a-138">Log upload status.</span></span> <span data-ttu-id="1d25a-139">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1d25a-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="1d25a-140">Ошибк</span><span class="sxs-lookup"><span data-stu-id="1d25a-140">errorMessage</span></span>|<span data-ttu-id="1d25a-141">String</span><span class="sxs-lookup"><span data-stu-id="1d25a-141">String</span></span>|<span data-ttu-id="1d25a-142">Сообщение об ошибке, если оно возникло во время процесса отправки</span><span class="sxs-lookup"><span data-stu-id="1d25a-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="1d25a-143">Кустомлогфолдерс</span><span class="sxs-lookup"><span data-stu-id="1d25a-143">customLogFolders</span></span>|<span data-ttu-id="1d25a-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1d25a-144">String collection</span></span>|<span data-ttu-id="1d25a-145">Список папок журналов.</span><span class="sxs-lookup"><span data-stu-id="1d25a-145">List of log folders.</span></span> |
|<span data-ttu-id="1d25a-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d25a-146">completedDateTime</span></span>|<span data-ttu-id="1d25a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d25a-147">DateTimeOffset</span></span>|<span data-ttu-id="1d25a-148">Время, когда запрос на отправку журнала достигает состояния терминала</span><span class="sxs-lookup"><span data-stu-id="1d25a-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="1d25a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d25a-149">Response</span></span>
<span data-ttu-id="1d25a-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d25a-150">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d25a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1d25a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d25a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d25a-152">Request</span></span>
<span data-ttu-id="1d25a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d25a-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d25a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d25a-154">Response</span></span>
<span data-ttu-id="1d25a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d25a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





