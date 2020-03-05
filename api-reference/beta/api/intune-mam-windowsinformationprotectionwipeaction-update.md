---
title: Обновление Виндовсинформатионпротектионвипеактион
description: Обновление свойств объекта Виндовсинформатионпротектионвипеактион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f82f7ba6d541f1a4a20721e7395b981659f5427
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462802"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="8c118-103">Обновление Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="8c118-103">Update windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="8c118-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c118-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c118-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c118-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c118-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c118-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c118-107">Обновление свойств объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="8c118-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c118-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c118-108">Prerequisites</span></span>
<span data-ttu-id="8c118-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c118-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c118-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c118-111">Permission type</span></span>|<span data-ttu-id="8c118-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c118-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c118-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c118-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c118-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c118-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c118-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c118-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c118-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c118-116">Not supported.</span></span>|
|<span data-ttu-id="8c118-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c118-117">Application</span></span>|<span data-ttu-id="8c118-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c118-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c118-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c118-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="8c118-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c118-120">Request headers</span></span>
|<span data-ttu-id="8c118-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c118-121">Header</span></span>|<span data-ttu-id="8c118-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c118-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c118-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c118-123">Authorization</span></span>|<span data-ttu-id="8c118-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c118-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c118-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c118-125">Accept</span></span>|<span data-ttu-id="8c118-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c118-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c118-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c118-127">Request body</span></span>
<span data-ttu-id="8c118-128">В тексте запроса добавьте представление объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c118-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="8c118-129">В следующей таблице приведены свойства, необходимые при создании [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="8c118-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="8c118-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c118-130">Property</span></span>|<span data-ttu-id="8c118-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c118-131">Type</span></span>|<span data-ttu-id="8c118-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c118-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c118-133">id</span><span class="sxs-lookup"><span data-stu-id="8c118-133">id</span></span>|<span data-ttu-id="8c118-134">String</span><span class="sxs-lookup"><span data-stu-id="8c118-134">String</span></span>|<span data-ttu-id="8c118-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c118-135">Key of the entity.</span></span>|
|<span data-ttu-id="8c118-136">status</span><span class="sxs-lookup"><span data-stu-id="8c118-136">status</span></span>|[<span data-ttu-id="8c118-137">actionState</span><span class="sxs-lookup"><span data-stu-id="8c118-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8c118-138">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="8c118-138">Wipe action status.</span></span> <span data-ttu-id="8c118-139">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8c118-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8c118-140">таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="8c118-140">targetedUserId</span></span>|<span data-ttu-id="8c118-141">String</span><span class="sxs-lookup"><span data-stu-id="8c118-141">String</span></span>|<span data-ttu-id="8c118-142">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="8c118-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="8c118-143">таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="8c118-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="8c118-144">String</span><span class="sxs-lookup"><span data-stu-id="8c118-144">String</span></span>|<span data-ttu-id="8c118-145">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="8c118-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="8c118-146">таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="8c118-146">targetedDeviceName</span></span>|<span data-ttu-id="8c118-147">String</span><span class="sxs-lookup"><span data-stu-id="8c118-147">String</span></span>|<span data-ttu-id="8c118-148">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="8c118-148">Targeted device name.</span></span>|
|<span data-ttu-id="8c118-149">таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="8c118-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="8c118-150">String</span><span class="sxs-lookup"><span data-stu-id="8c118-150">String</span></span>|<span data-ttu-id="8c118-151">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="8c118-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="8c118-152">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="8c118-152">lastCheckInDateTime</span></span>|<span data-ttu-id="8c118-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c118-153">DateTimeOffset</span></span>|<span data-ttu-id="8c118-154">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="8c118-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="8c118-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c118-155">Response</span></span>
<span data-ttu-id="8c118-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c118-156">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c118-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8c118-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c118-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c118-158">Request</span></span>
<span data-ttu-id="8c118-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c118-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c118-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c118-160">Response</span></span>
<span data-ttu-id="8c118-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c118-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





