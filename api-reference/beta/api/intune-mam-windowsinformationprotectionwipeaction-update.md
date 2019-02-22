---
title: Обновление Виндовсинформатионпротектионвипеактион
description: Обновление свойств объекта Виндовсинформатионпротектионвипеактион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b198f1387cc3f0806cc6b76953948eca08d88cfc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159103"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="19bf2-103">Обновление Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="19bf2-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="19bf2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19bf2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19bf2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19bf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19bf2-106">Обновление свойств объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="19bf2-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19bf2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19bf2-107">Prerequisites</span></span>
<span data-ttu-id="19bf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19bf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19bf2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19bf2-110">Permission type</span></span>|<span data-ttu-id="19bf2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19bf2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19bf2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19bf2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19bf2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19bf2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19bf2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19bf2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19bf2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19bf2-115">Not supported.</span></span>|
|<span data-ttu-id="19bf2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19bf2-116">Application</span></span>|<span data-ttu-id="19bf2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19bf2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19bf2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19bf2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="19bf2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19bf2-119">Request headers</span></span>
|<span data-ttu-id="19bf2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19bf2-120">Header</span></span>|<span data-ttu-id="19bf2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19bf2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19bf2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19bf2-122">Authorization</span></span>|<span data-ttu-id="19bf2-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19bf2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19bf2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="19bf2-124">Accept</span></span>|<span data-ttu-id="19bf2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19bf2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19bf2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19bf2-126">Request body</span></span>
<span data-ttu-id="19bf2-127">В тексте запроса добавьте представление объекта [Виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19bf2-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="19bf2-128">В следующей таблице приведены свойства, необходимые при создании [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="19bf2-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="19bf2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="19bf2-129">Property</span></span>|<span data-ttu-id="19bf2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="19bf2-130">Type</span></span>|<span data-ttu-id="19bf2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="19bf2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19bf2-132">id</span><span class="sxs-lookup"><span data-stu-id="19bf2-132">id</span></span>|<span data-ttu-id="19bf2-133">String</span><span class="sxs-lookup"><span data-stu-id="19bf2-133">String</span></span>|<span data-ttu-id="19bf2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19bf2-134">Key of the entity.</span></span>|
|<span data-ttu-id="19bf2-135">status</span><span class="sxs-lookup"><span data-stu-id="19bf2-135">status</span></span>|[<span data-ttu-id="19bf2-136">actionState</span><span class="sxs-lookup"><span data-stu-id="19bf2-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="19bf2-137">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="19bf2-137">Wipe action status.</span></span> <span data-ttu-id="19bf2-138">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="19bf2-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="19bf2-139">Таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="19bf2-139">targetedUserId</span></span>|<span data-ttu-id="19bf2-140">String</span><span class="sxs-lookup"><span data-stu-id="19bf2-140">String</span></span>|<span data-ttu-id="19bf2-141">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="19bf2-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="19bf2-142">Таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="19bf2-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="19bf2-143">String</span><span class="sxs-lookup"><span data-stu-id="19bf2-143">String</span></span>|<span data-ttu-id="19bf2-144">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="19bf2-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="19bf2-145">Таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="19bf2-145">targetedDeviceName</span></span>|<span data-ttu-id="19bf2-146">String</span><span class="sxs-lookup"><span data-stu-id="19bf2-146">String</span></span>|<span data-ttu-id="19bf2-147">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="19bf2-147">Targeted device name.</span></span>|
|<span data-ttu-id="19bf2-148">Таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="19bf2-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="19bf2-149">String</span><span class="sxs-lookup"><span data-stu-id="19bf2-149">String</span></span>|<span data-ttu-id="19bf2-150">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="19bf2-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="19bf2-151">Ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="19bf2-151">lastCheckInDateTime</span></span>|<span data-ttu-id="19bf2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19bf2-152">DateTimeOffset</span></span>|<span data-ttu-id="19bf2-153">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="19bf2-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="19bf2-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="19bf2-154">Response</span></span>
<span data-ttu-id="19bf2-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19bf2-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19bf2-156">Пример</span><span class="sxs-lookup"><span data-stu-id="19bf2-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="19bf2-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="19bf2-157">Request</span></span>
<span data-ttu-id="19bf2-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19bf2-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19bf2-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="19bf2-159">Response</span></span>
<span data-ttu-id="19bf2-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19bf2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




