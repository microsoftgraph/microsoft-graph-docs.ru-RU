---
title: Создание Виндовсинформатионпротектионвипеактион
description: Создание нового объекта Виндовсинформатионпротектионвипеактион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24e0d2863c0b9a038bf3667ab42fe4a392d49729
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981526"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="30a25-103">Создание Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="30a25-103">Create windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="30a25-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30a25-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30a25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30a25-106">Создание нового объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="30a25-106">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30a25-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30a25-107">Prerequisites</span></span>
<span data-ttu-id="30a25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a25-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30a25-110">Permission type</span></span>|<span data-ttu-id="30a25-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30a25-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30a25-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30a25-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30a25-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a25-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30a25-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30a25-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30a25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a25-115">Not supported.</span></span>|
|<span data-ttu-id="30a25-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30a25-116">Application</span></span>|<span data-ttu-id="30a25-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a25-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30a25-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30a25-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="30a25-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30a25-119">Request headers</span></span>
|<span data-ttu-id="30a25-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30a25-120">Header</span></span>|<span data-ttu-id="30a25-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30a25-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30a25-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30a25-122">Authorization</span></span>|<span data-ttu-id="30a25-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30a25-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30a25-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30a25-124">Accept</span></span>|<span data-ttu-id="30a25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30a25-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30a25-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30a25-126">Request body</span></span>
<span data-ttu-id="30a25-127">В тексте запроса добавьте представление объекта Виндовсинформатионпротектионвипеактион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a25-127">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="30a25-128">В следующей таблице приведены свойства, необходимые при создании Виндовсинформатионпротектионвипеактион.</span><span class="sxs-lookup"><span data-stu-id="30a25-128">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="30a25-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30a25-129">Property</span></span>|<span data-ttu-id="30a25-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30a25-130">Type</span></span>|<span data-ttu-id="30a25-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30a25-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30a25-132">id</span><span class="sxs-lookup"><span data-stu-id="30a25-132">id</span></span>|<span data-ttu-id="30a25-133">String</span><span class="sxs-lookup"><span data-stu-id="30a25-133">String</span></span>|<span data-ttu-id="30a25-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30a25-134">Key of the entity.</span></span>|
|<span data-ttu-id="30a25-135">status</span><span class="sxs-lookup"><span data-stu-id="30a25-135">status</span></span>|[<span data-ttu-id="30a25-136">actionState</span><span class="sxs-lookup"><span data-stu-id="30a25-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="30a25-137">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="30a25-137">Wipe action status.</span></span> <span data-ttu-id="30a25-138">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="30a25-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="30a25-139">Таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="30a25-139">targetedUserId</span></span>|<span data-ttu-id="30a25-140">String</span><span class="sxs-lookup"><span data-stu-id="30a25-140">String</span></span>|<span data-ttu-id="30a25-141">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="30a25-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="30a25-142">Таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="30a25-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="30a25-143">String</span><span class="sxs-lookup"><span data-stu-id="30a25-143">String</span></span>|<span data-ttu-id="30a25-144">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="30a25-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="30a25-145">Таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="30a25-145">targetedDeviceName</span></span>|<span data-ttu-id="30a25-146">String</span><span class="sxs-lookup"><span data-stu-id="30a25-146">String</span></span>|<span data-ttu-id="30a25-147">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="30a25-147">Targeted device name.</span></span>|
|<span data-ttu-id="30a25-148">Таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="30a25-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="30a25-149">String</span><span class="sxs-lookup"><span data-stu-id="30a25-149">String</span></span>|<span data-ttu-id="30a25-150">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="30a25-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="30a25-151">Ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="30a25-151">lastCheckInDateTime</span></span>|<span data-ttu-id="30a25-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30a25-152">DateTimeOffset</span></span>|<span data-ttu-id="30a25-153">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="30a25-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="30a25-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a25-154">Response</span></span>
<span data-ttu-id="30a25-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30a25-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a25-156">Пример</span><span class="sxs-lookup"><span data-stu-id="30a25-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="30a25-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a25-157">Request</span></span>
<span data-ttu-id="30a25-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30a25-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30a25-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a25-159">Response</span></span>
<span data-ttu-id="30a25-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30a25-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





