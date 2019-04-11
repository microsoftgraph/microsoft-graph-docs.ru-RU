---
title: Обновление Виндовсинформатионпротектионвипеактион
description: Обновление свойств объекта Виндовсинформатионпротектионвипеактион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e59eeb987e678764adcd5f4378f6bfdc5b4907e0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777608"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="4b0cc-103">Обновление Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="4b0cc-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="4b0cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b0cc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b0cc-106">Обновление свойств объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="4b0cc-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b0cc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b0cc-107">Prerequisites</span></span>
<span data-ttu-id="4b0cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b0cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b0cc-110">Permission type</span></span>|<span data-ttu-id="4b0cc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b0cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b0cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b0cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b0cc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0cc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b0cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b0cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b0cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-115">Not supported.</span></span>|
|<span data-ttu-id="4b0cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b0cc-116">Application</span></span>|<span data-ttu-id="4b0cc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b0cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b0cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="4b0cc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b0cc-119">Request headers</span></span>
|<span data-ttu-id="4b0cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b0cc-120">Header</span></span>|<span data-ttu-id="4b0cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b0cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b0cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b0cc-122">Authorization</span></span>|<span data-ttu-id="4b0cc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b0cc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b0cc-124">Accept</span></span>|<span data-ttu-id="4b0cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b0cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b0cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b0cc-126">Request body</span></span>
<span data-ttu-id="4b0cc-127">В тексте запроса добавьте представление объекта [Виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="4b0cc-128">В следующей таблице приведены свойства, необходимые при создании [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="4b0cc-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="4b0cc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b0cc-129">Property</span></span>|<span data-ttu-id="4b0cc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b0cc-130">Type</span></span>|<span data-ttu-id="4b0cc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b0cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b0cc-132">id</span><span class="sxs-lookup"><span data-stu-id="4b0cc-132">id</span></span>|<span data-ttu-id="4b0cc-133">String</span><span class="sxs-lookup"><span data-stu-id="4b0cc-133">String</span></span>|<span data-ttu-id="4b0cc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-134">Key of the entity.</span></span>|
|<span data-ttu-id="4b0cc-135">status</span><span class="sxs-lookup"><span data-stu-id="4b0cc-135">status</span></span>|[<span data-ttu-id="4b0cc-136">actionState</span><span class="sxs-lookup"><span data-stu-id="4b0cc-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4b0cc-137">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-137">Wipe action status.</span></span> <span data-ttu-id="4b0cc-138">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4b0cc-139">Таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="4b0cc-139">targetedUserId</span></span>|<span data-ttu-id="4b0cc-140">String</span><span class="sxs-lookup"><span data-stu-id="4b0cc-140">String</span></span>|<span data-ttu-id="4b0cc-141">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="4b0cc-142">Таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="4b0cc-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="4b0cc-143">String</span><span class="sxs-lookup"><span data-stu-id="4b0cc-143">String</span></span>|<span data-ttu-id="4b0cc-144">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="4b0cc-145">Таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="4b0cc-145">targetedDeviceName</span></span>|<span data-ttu-id="4b0cc-146">String</span><span class="sxs-lookup"><span data-stu-id="4b0cc-146">String</span></span>|<span data-ttu-id="4b0cc-147">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-147">Targeted device name.</span></span>|
|<span data-ttu-id="4b0cc-148">Таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="4b0cc-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="4b0cc-149">String</span><span class="sxs-lookup"><span data-stu-id="4b0cc-149">String</span></span>|<span data-ttu-id="4b0cc-150">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="4b0cc-151">Ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="4b0cc-151">lastCheckInDateTime</span></span>|<span data-ttu-id="4b0cc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b0cc-152">DateTimeOffset</span></span>|<span data-ttu-id="4b0cc-153">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="4b0cc-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0cc-154">Response</span></span>
<span data-ttu-id="4b0cc-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0cc-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4b0cc-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b0cc-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b0cc-157">Request</span></span>
<span data-ttu-id="4b0cc-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b0cc-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0cc-159">Response</span></span>
<span data-ttu-id="4b0cc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b0cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





