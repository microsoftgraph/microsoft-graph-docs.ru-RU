---
title: Создание windowsInformationProtectionWipeAction
description: Создание нового объекта windowsInformationProtectionWipeAction.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9bee06b2221a80a303d2754568e31b09e6c5adec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141871"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="71453-103">Создание windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="71453-103">Create windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="71453-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71453-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71453-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71453-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71453-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71453-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71453-107">Создание нового [объекта windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)</span><span class="sxs-lookup"><span data-stu-id="71453-107">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71453-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71453-108">Prerequisites</span></span>
<span data-ttu-id="71453-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71453-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71453-111">Permission type</span></span>|<span data-ttu-id="71453-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71453-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71453-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71453-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71453-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71453-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71453-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71453-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71453-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71453-116">Not supported.</span></span>|
|<span data-ttu-id="71453-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="71453-117">Application</span></span>|<span data-ttu-id="71453-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71453-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71453-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71453-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="71453-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71453-120">Request headers</span></span>
|<span data-ttu-id="71453-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71453-121">Header</span></span>|<span data-ttu-id="71453-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71453-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71453-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71453-123">Authorization</span></span>|<span data-ttu-id="71453-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71453-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71453-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71453-125">Accept</span></span>|<span data-ttu-id="71453-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71453-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71453-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71453-127">Request body</span></span>
<span data-ttu-id="71453-128">В теле запроса поставляем представление JSON для объекта windowsInformationProtectionWipeAction.</span><span class="sxs-lookup"><span data-stu-id="71453-128">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="71453-129">В следующей таблице показаны свойства, необходимые при создании windowsInformationProtectionWipeAction.</span><span class="sxs-lookup"><span data-stu-id="71453-129">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="71453-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71453-130">Property</span></span>|<span data-ttu-id="71453-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71453-131">Type</span></span>|<span data-ttu-id="71453-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71453-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71453-133">id</span><span class="sxs-lookup"><span data-stu-id="71453-133">id</span></span>|<span data-ttu-id="71453-134">Строка</span><span class="sxs-lookup"><span data-stu-id="71453-134">String</span></span>|<span data-ttu-id="71453-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71453-135">Key of the entity.</span></span>|
|<span data-ttu-id="71453-136">status</span><span class="sxs-lookup"><span data-stu-id="71453-136">status</span></span>|[<span data-ttu-id="71453-137">actionState</span><span class="sxs-lookup"><span data-stu-id="71453-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="71453-138">Wipe action status.</span><span class="sxs-lookup"><span data-stu-id="71453-138">Wipe action status.</span></span> <span data-ttu-id="71453-139">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="71453-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="71453-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="71453-140">targetedUserId</span></span>|<span data-ttu-id="71453-141">Строка</span><span class="sxs-lookup"><span data-stu-id="71453-141">String</span></span>|<span data-ttu-id="71453-142">Объект UserId, на который нацелено это действие стирки.</span><span class="sxs-lookup"><span data-stu-id="71453-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="71453-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="71453-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="71453-144">Строка</span><span class="sxs-lookup"><span data-stu-id="71453-144">String</span></span>|<span data-ttu-id="71453-145">Объект DeviceRegistrationId, нацеленный этим действием на стирку.</span><span class="sxs-lookup"><span data-stu-id="71453-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="71453-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="71453-146">targetedDeviceName</span></span>|<span data-ttu-id="71453-147">Строка</span><span class="sxs-lookup"><span data-stu-id="71453-147">String</span></span>|<span data-ttu-id="71453-148">Целевое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="71453-148">Targeted device name.</span></span>|
|<span data-ttu-id="71453-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="71453-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="71453-150">Строка</span><span class="sxs-lookup"><span data-stu-id="71453-150">String</span></span>|<span data-ttu-id="71453-151">Адрес Mac целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="71453-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="71453-152">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="71453-152">lastCheckInDateTime</span></span>|<span data-ttu-id="71453-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71453-153">DateTimeOffset</span></span>|<span data-ttu-id="71453-154">Время последней проверки устройства, на которое было нацелено это действие стирки.</span><span class="sxs-lookup"><span data-stu-id="71453-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="71453-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="71453-155">Response</span></span>
<span data-ttu-id="71453-156">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71453-156">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71453-157">Пример</span><span class="sxs-lookup"><span data-stu-id="71453-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="71453-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="71453-158">Request</span></span>
<span data-ttu-id="71453-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71453-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="71453-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="71453-160">Response</span></span>
<span data-ttu-id="71453-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71453-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




