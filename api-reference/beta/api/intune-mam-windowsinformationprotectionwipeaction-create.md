---
title: Создание Виндовсинформатионпротектионвипеактион
description: Создание нового объекта Виндовсинформатионпротектионвипеактион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 936f0edcbf41fb9556ab8c67dbbd41da42b211dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353388"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="bf3b9-103">Создание Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="bf3b9-103">Create windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="bf3b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf3b9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf3b9-106">Создание нового объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="bf3b9-106">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf3b9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf3b9-107">Prerequisites</span></span>
<span data-ttu-id="bf3b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf3b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf3b9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf3b9-110">Permission type</span></span>|<span data-ttu-id="bf3b9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf3b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf3b9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf3b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf3b9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf3b9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bf3b9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf3b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf3b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-115">Not supported.</span></span>|
|<span data-ttu-id="bf3b9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf3b9-116">Application</span></span>|<span data-ttu-id="bf3b9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf3b9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf3b9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf3b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="bf3b9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf3b9-119">Request headers</span></span>
|<span data-ttu-id="bf3b9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf3b9-120">Header</span></span>|<span data-ttu-id="bf3b9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf3b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf3b9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf3b9-122">Authorization</span></span>|<span data-ttu-id="bf3b9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf3b9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf3b9-124">Accept</span></span>|<span data-ttu-id="bf3b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf3b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf3b9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf3b9-126">Request body</span></span>
<span data-ttu-id="bf3b9-127">В тексте запроса добавьте представление объекта Виндовсинформатионпротектионвипеактион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-127">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="bf3b9-128">В следующей таблице приведены свойства, необходимые при создании Виндовсинформатионпротектионвипеактион.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-128">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="bf3b9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf3b9-129">Property</span></span>|<span data-ttu-id="bf3b9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf3b9-130">Type</span></span>|<span data-ttu-id="bf3b9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf3b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf3b9-132">id</span><span class="sxs-lookup"><span data-stu-id="bf3b9-132">id</span></span>|<span data-ttu-id="bf3b9-133">String</span><span class="sxs-lookup"><span data-stu-id="bf3b9-133">String</span></span>|<span data-ttu-id="bf3b9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-134">Key of the entity.</span></span>|
|<span data-ttu-id="bf3b9-135">status</span><span class="sxs-lookup"><span data-stu-id="bf3b9-135">status</span></span>|[<span data-ttu-id="bf3b9-136">actionState</span><span class="sxs-lookup"><span data-stu-id="bf3b9-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bf3b9-137">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-137">Wipe action status.</span></span> <span data-ttu-id="bf3b9-138">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bf3b9-139">таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="bf3b9-139">targetedUserId</span></span>|<span data-ttu-id="bf3b9-140">String</span><span class="sxs-lookup"><span data-stu-id="bf3b9-140">String</span></span>|<span data-ttu-id="bf3b9-141">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="bf3b9-142">таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="bf3b9-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="bf3b9-143">String</span><span class="sxs-lookup"><span data-stu-id="bf3b9-143">String</span></span>|<span data-ttu-id="bf3b9-144">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="bf3b9-145">таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="bf3b9-145">targetedDeviceName</span></span>|<span data-ttu-id="bf3b9-146">String</span><span class="sxs-lookup"><span data-stu-id="bf3b9-146">String</span></span>|<span data-ttu-id="bf3b9-147">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-147">Targeted device name.</span></span>|
|<span data-ttu-id="bf3b9-148">таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="bf3b9-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="bf3b9-149">String</span><span class="sxs-lookup"><span data-stu-id="bf3b9-149">String</span></span>|<span data-ttu-id="bf3b9-150">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="bf3b9-151">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="bf3b9-151">lastCheckInDateTime</span></span>|<span data-ttu-id="bf3b9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf3b9-152">DateTimeOffset</span></span>|<span data-ttu-id="bf3b9-153">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="bf3b9-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3b9-154">Response</span></span>
<span data-ttu-id="bf3b9-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf3b9-156">Пример</span><span class="sxs-lookup"><span data-stu-id="bf3b9-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf3b9-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf3b9-157">Request</span></span>
<span data-ttu-id="bf3b9-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bf3b9-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3b9-159">Response</span></span>
<span data-ttu-id="bf3b9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf3b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






