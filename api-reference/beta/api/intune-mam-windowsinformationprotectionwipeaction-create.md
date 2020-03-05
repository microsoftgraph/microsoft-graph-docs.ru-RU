---
title: Создание Виндовсинформатионпротектионвипеактион
description: Создание нового объекта Виндовсинформатионпротектионвипеактион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bffa30178e881ccb30cefab218d53df5e0cd639
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462812"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="4ac80-103">Создание Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="4ac80-103">Create windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="4ac80-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ac80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ac80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ac80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ac80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ac80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ac80-107">Создание нового объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="4ac80-107">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ac80-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ac80-108">Prerequisites</span></span>
<span data-ttu-id="4ac80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ac80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ac80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ac80-111">Permission type</span></span>|<span data-ttu-id="4ac80-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ac80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ac80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ac80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ac80-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac80-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4ac80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ac80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ac80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ac80-116">Not supported.</span></span>|
|<span data-ttu-id="4ac80-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ac80-117">Application</span></span>|<span data-ttu-id="4ac80-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac80-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ac80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ac80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="4ac80-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ac80-120">Request headers</span></span>
|<span data-ttu-id="4ac80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ac80-121">Header</span></span>|<span data-ttu-id="4ac80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ac80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ac80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ac80-123">Authorization</span></span>|<span data-ttu-id="4ac80-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ac80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ac80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ac80-125">Accept</span></span>|<span data-ttu-id="4ac80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ac80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ac80-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ac80-127">Request body</span></span>
<span data-ttu-id="4ac80-128">В тексте запроса добавьте представление объекта Виндовсинформатионпротектионвипеактион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ac80-128">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="4ac80-129">В следующей таблице приведены свойства, необходимые при создании Виндовсинформатионпротектионвипеактион.</span><span class="sxs-lookup"><span data-stu-id="4ac80-129">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="4ac80-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ac80-130">Property</span></span>|<span data-ttu-id="4ac80-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4ac80-131">Type</span></span>|<span data-ttu-id="4ac80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4ac80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ac80-133">id</span><span class="sxs-lookup"><span data-stu-id="4ac80-133">id</span></span>|<span data-ttu-id="4ac80-134">String</span><span class="sxs-lookup"><span data-stu-id="4ac80-134">String</span></span>|<span data-ttu-id="4ac80-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4ac80-135">Key of the entity.</span></span>|
|<span data-ttu-id="4ac80-136">status</span><span class="sxs-lookup"><span data-stu-id="4ac80-136">status</span></span>|[<span data-ttu-id="4ac80-137">actionState</span><span class="sxs-lookup"><span data-stu-id="4ac80-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4ac80-138">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4ac80-138">Wipe action status.</span></span> <span data-ttu-id="4ac80-139">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4ac80-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4ac80-140">таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="4ac80-140">targetedUserId</span></span>|<span data-ttu-id="4ac80-141">String</span><span class="sxs-lookup"><span data-stu-id="4ac80-141">String</span></span>|<span data-ttu-id="4ac80-142">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4ac80-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="4ac80-143">таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="4ac80-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="4ac80-144">String</span><span class="sxs-lookup"><span data-stu-id="4ac80-144">String</span></span>|<span data-ttu-id="4ac80-145">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4ac80-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="4ac80-146">таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="4ac80-146">targetedDeviceName</span></span>|<span data-ttu-id="4ac80-147">String</span><span class="sxs-lookup"><span data-stu-id="4ac80-147">String</span></span>|<span data-ttu-id="4ac80-148">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="4ac80-148">Targeted device name.</span></span>|
|<span data-ttu-id="4ac80-149">таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="4ac80-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="4ac80-150">String</span><span class="sxs-lookup"><span data-stu-id="4ac80-150">String</span></span>|<span data-ttu-id="4ac80-151">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="4ac80-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="4ac80-152">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="4ac80-152">lastCheckInDateTime</span></span>|<span data-ttu-id="4ac80-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ac80-153">DateTimeOffset</span></span>|<span data-ttu-id="4ac80-154">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4ac80-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="4ac80-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ac80-155">Response</span></span>
<span data-ttu-id="4ac80-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ac80-156">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ac80-157">Пример</span><span class="sxs-lookup"><span data-stu-id="4ac80-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ac80-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ac80-158">Request</span></span>
<span data-ttu-id="4ac80-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ac80-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ac80-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ac80-160">Response</span></span>
<span data-ttu-id="4ac80-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ac80-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





