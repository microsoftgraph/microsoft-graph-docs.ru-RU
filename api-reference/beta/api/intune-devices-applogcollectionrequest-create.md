---
title: Создание appLogCollectionRequest
description: Создание нового объекта appLogCollectionRequest.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c3afd1cf00ba706e3fbc1e960e649fc010ae582f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430770"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="4b01d-103">Создание appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="4b01d-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="4b01d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b01d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b01d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b01d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b01d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b01d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b01d-107">Создание нового объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4b01d-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b01d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4b01d-108">Prerequisites</span></span>
<span data-ttu-id="4b01d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b01d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b01d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b01d-111">Permission type</span></span>|<span data-ttu-id="4b01d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b01d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b01d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b01d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b01d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b01d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4b01d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b01d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b01d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b01d-116">Not supported.</span></span>|
|<span data-ttu-id="4b01d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b01d-117">Application</span></span>|<span data-ttu-id="4b01d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b01d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b01d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b01d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="4b01d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b01d-120">Request headers</span></span>
|<span data-ttu-id="4b01d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b01d-121">Header</span></span>|<span data-ttu-id="4b01d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b01d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b01d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b01d-123">Authorization</span></span>|<span data-ttu-id="4b01d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4b01d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b01d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b01d-125">Accept</span></span>|<span data-ttu-id="4b01d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b01d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b01d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b01d-127">Request body</span></span>
<span data-ttu-id="4b01d-128">В тексте запроса укажите представление JSON для объекта appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="4b01d-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="4b01d-129">В следующей таблице показаны свойства, которые необходимы для создания appLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="4b01d-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="4b01d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b01d-130">Property</span></span>|<span data-ttu-id="4b01d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b01d-131">Type</span></span>|<span data-ttu-id="4b01d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b01d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b01d-133">id</span><span class="sxs-lookup"><span data-stu-id="4b01d-133">id</span></span>|<span data-ttu-id="4b01d-134">String</span><span class="sxs-lookup"><span data-stu-id="4b01d-134">String</span></span>|<span data-ttu-id="4b01d-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4b01d-135">The unique Identifier.</span></span> <span data-ttu-id="4b01d-136">— Идентификатор userId_DeviceId_AppId.</span><span class="sxs-lookup"><span data-stu-id="4b01d-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="4b01d-137">status</span><span class="sxs-lookup"><span data-stu-id="4b01d-137">status</span></span>|[<span data-ttu-id="4b01d-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="4b01d-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="4b01d-139">Статус отправки журнала.</span><span class="sxs-lookup"><span data-stu-id="4b01d-139">Log upload status.</span></span> <span data-ttu-id="4b01d-140">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4b01d-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="4b01d-141">сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="4b01d-141">errorMessage</span></span>|<span data-ttu-id="4b01d-142">String</span><span class="sxs-lookup"><span data-stu-id="4b01d-142">String</span></span>|<span data-ttu-id="4b01d-143">Сообщение об ошибке, если они существуют в процессе загрузки</span><span class="sxs-lookup"><span data-stu-id="4b01d-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="4b01d-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="4b01d-144">customLogFolders</span></span>|<span data-ttu-id="4b01d-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b01d-145">String collection</span></span>|<span data-ttu-id="4b01d-146">Список папок, журнала.</span><span class="sxs-lookup"><span data-stu-id="4b01d-146">List of log folders.</span></span> |
|<span data-ttu-id="4b01d-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b01d-147">completedDateTime</span></span>|<span data-ttu-id="4b01d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b01d-148">DateTimeOffset</span></span>|<span data-ttu-id="4b01d-149">Время, в которой запроса журнала загрузки связаться с вами состоянии</span><span class="sxs-lookup"><span data-stu-id="4b01d-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="4b01d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b01d-150">Response</span></span>
<span data-ttu-id="4b01d-151">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b01d-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b01d-152">Пример</span><span class="sxs-lookup"><span data-stu-id="4b01d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b01d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b01d-153">Request</span></span>
<span data-ttu-id="4b01d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b01d-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b01d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b01d-155">Response</span></span>
<span data-ttu-id="4b01d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b01d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




