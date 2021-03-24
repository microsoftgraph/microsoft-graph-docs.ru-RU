---
title: Обновление windowsInformationProtectionWipeAction
description: Обновление свойств объекта windowsInformationProtectionWipeAction.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b2df26a5aa357d1ebfe6a125049e3a69b1022ae
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141808"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="40ae0-103">Обновление windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="40ae0-103">Update windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="40ae0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ae0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40ae0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ae0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40ae0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40ae0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40ae0-107">Обновление свойств объекта [windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)</span><span class="sxs-lookup"><span data-stu-id="40ae0-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40ae0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="40ae0-108">Prerequisites</span></span>
<span data-ttu-id="40ae0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ae0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40ae0-111">Permission type</span></span>|<span data-ttu-id="40ae0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40ae0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ae0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40ae0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40ae0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ae0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40ae0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40ae0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40ae0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ae0-116">Not supported.</span></span>|
|<span data-ttu-id="40ae0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="40ae0-117">Application</span></span>|<span data-ttu-id="40ae0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ae0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40ae0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40ae0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="40ae0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40ae0-120">Request headers</span></span>
|<span data-ttu-id="40ae0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40ae0-121">Header</span></span>|<span data-ttu-id="40ae0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40ae0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40ae0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ae0-123">Authorization</span></span>|<span data-ttu-id="40ae0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ae0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40ae0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40ae0-125">Accept</span></span>|<span data-ttu-id="40ae0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40ae0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ae0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40ae0-127">Request body</span></span>
<span data-ttu-id="40ae0-128">В теле запроса поставляем представление JSON для [объекта windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)</span><span class="sxs-lookup"><span data-stu-id="40ae0-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="40ae0-129">В следующей таблице показаны свойства, необходимые при создании [windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)</span><span class="sxs-lookup"><span data-stu-id="40ae0-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="40ae0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="40ae0-130">Property</span></span>|<span data-ttu-id="40ae0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40ae0-131">Type</span></span>|<span data-ttu-id="40ae0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40ae0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40ae0-133">id</span><span class="sxs-lookup"><span data-stu-id="40ae0-133">id</span></span>|<span data-ttu-id="40ae0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="40ae0-134">String</span></span>|<span data-ttu-id="40ae0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="40ae0-135">Key of the entity.</span></span>|
|<span data-ttu-id="40ae0-136">status</span><span class="sxs-lookup"><span data-stu-id="40ae0-136">status</span></span>|[<span data-ttu-id="40ae0-137">actionState</span><span class="sxs-lookup"><span data-stu-id="40ae0-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="40ae0-138">Wipe action status.</span><span class="sxs-lookup"><span data-stu-id="40ae0-138">Wipe action status.</span></span> <span data-ttu-id="40ae0-139">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="40ae0-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="40ae0-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="40ae0-140">targetedUserId</span></span>|<span data-ttu-id="40ae0-141">Строка</span><span class="sxs-lookup"><span data-stu-id="40ae0-141">String</span></span>|<span data-ttu-id="40ae0-142">Объект UserId, на который нацелено это действие стирки.</span><span class="sxs-lookup"><span data-stu-id="40ae0-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="40ae0-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="40ae0-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="40ae0-144">Строка</span><span class="sxs-lookup"><span data-stu-id="40ae0-144">String</span></span>|<span data-ttu-id="40ae0-145">Объект DeviceRegistrationId, нацеленный этим действием на стирку.</span><span class="sxs-lookup"><span data-stu-id="40ae0-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="40ae0-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="40ae0-146">targetedDeviceName</span></span>|<span data-ttu-id="40ae0-147">Строка</span><span class="sxs-lookup"><span data-stu-id="40ae0-147">String</span></span>|<span data-ttu-id="40ae0-148">Целевое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="40ae0-148">Targeted device name.</span></span>|
|<span data-ttu-id="40ae0-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="40ae0-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="40ae0-150">Строка</span><span class="sxs-lookup"><span data-stu-id="40ae0-150">String</span></span>|<span data-ttu-id="40ae0-151">Адрес Mac целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="40ae0-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="40ae0-152">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="40ae0-152">lastCheckInDateTime</span></span>|<span data-ttu-id="40ae0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40ae0-153">DateTimeOffset</span></span>|<span data-ttu-id="40ae0-154">Время последней проверки устройства, на которое было нацелено это действие стирки.</span><span class="sxs-lookup"><span data-stu-id="40ae0-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="40ae0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ae0-155">Response</span></span>
<span data-ttu-id="40ae0-156">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40ae0-156">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ae0-157">Пример</span><span class="sxs-lookup"><span data-stu-id="40ae0-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="40ae0-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="40ae0-158">Request</span></span>
<span data-ttu-id="40ae0-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40ae0-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
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

### <a name="response"></a><span data-ttu-id="40ae0-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ae0-160">Response</span></span>
<span data-ttu-id="40ae0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40ae0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




