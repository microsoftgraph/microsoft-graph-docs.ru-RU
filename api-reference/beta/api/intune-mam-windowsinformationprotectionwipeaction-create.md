---
title: Создание Виндовсинформатионпротектионвипеактион
description: Создание нового объекта Виндовсинформатионпротектионвипеактион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82baaab62e9f9f4ad20e97220cc701aebbbdb9eb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685088"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="efbac-103">Создание Виндовсинформатионпротектионвипеактион</span><span class="sxs-lookup"><span data-stu-id="efbac-103">Create windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="efbac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efbac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efbac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efbac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efbac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efbac-107">Создание нового объекта [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="efbac-107">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efbac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="efbac-108">Prerequisites</span></span>
<span data-ttu-id="efbac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efbac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efbac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efbac-111">Permission type</span></span>|<span data-ttu-id="efbac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efbac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efbac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efbac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efbac-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbac-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="efbac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efbac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efbac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbac-116">Not supported.</span></span>|
|<span data-ttu-id="efbac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efbac-117">Application</span></span>|<span data-ttu-id="efbac-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbac-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efbac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efbac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="efbac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efbac-120">Request headers</span></span>
|<span data-ttu-id="efbac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efbac-121">Header</span></span>|<span data-ttu-id="efbac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="efbac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efbac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efbac-123">Authorization</span></span>|<span data-ttu-id="efbac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efbac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efbac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efbac-125">Accept</span></span>|<span data-ttu-id="efbac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efbac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efbac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="efbac-127">Request body</span></span>
<span data-ttu-id="efbac-128">В тексте запроса добавьте представление объекта Виндовсинформатионпротектионвипеактион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efbac-128">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="efbac-129">В следующей таблице приведены свойства, необходимые при создании Виндовсинформатионпротектионвипеактион.</span><span class="sxs-lookup"><span data-stu-id="efbac-129">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="efbac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="efbac-130">Property</span></span>|<span data-ttu-id="efbac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="efbac-131">Type</span></span>|<span data-ttu-id="efbac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="efbac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efbac-133">id</span><span class="sxs-lookup"><span data-stu-id="efbac-133">id</span></span>|<span data-ttu-id="efbac-134">Строка</span><span class="sxs-lookup"><span data-stu-id="efbac-134">String</span></span>|<span data-ttu-id="efbac-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="efbac-135">Key of the entity.</span></span>|
|<span data-ttu-id="efbac-136">status</span><span class="sxs-lookup"><span data-stu-id="efbac-136">status</span></span>|[<span data-ttu-id="efbac-137">actionState</span><span class="sxs-lookup"><span data-stu-id="efbac-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="efbac-138">Состояние действия очистки.</span><span class="sxs-lookup"><span data-stu-id="efbac-138">Wipe action status.</span></span> <span data-ttu-id="efbac-139">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="efbac-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="efbac-140">таржетедусерид</span><span class="sxs-lookup"><span data-stu-id="efbac-140">targetedUserId</span></span>|<span data-ttu-id="efbac-141">Строка</span><span class="sxs-lookup"><span data-stu-id="efbac-141">String</span></span>|<span data-ttu-id="efbac-142">UserId, целевой для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="efbac-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="efbac-143">таржетеддевицерегистратионид</span><span class="sxs-lookup"><span data-stu-id="efbac-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="efbac-144">Строка</span><span class="sxs-lookup"><span data-stu-id="efbac-144">String</span></span>|<span data-ttu-id="efbac-145">Девицерегистратионид, предназначенный для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="efbac-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="efbac-146">таржетеддевиценаме</span><span class="sxs-lookup"><span data-stu-id="efbac-146">targetedDeviceName</span></span>|<span data-ttu-id="efbac-147">Строка</span><span class="sxs-lookup"><span data-stu-id="efbac-147">String</span></span>|<span data-ttu-id="efbac-148">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="efbac-148">Targeted device name.</span></span>|
|<span data-ttu-id="efbac-149">таржетеддевицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="efbac-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="efbac-150">Строка</span><span class="sxs-lookup"><span data-stu-id="efbac-150">String</span></span>|<span data-ttu-id="efbac-151">Mac-адрес целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="efbac-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="efbac-152">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="efbac-152">lastCheckInDateTime</span></span>|<span data-ttu-id="efbac-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efbac-153">DateTimeOffset</span></span>|<span data-ttu-id="efbac-154">Время последнего возврата устройства, которое было назначено для этого действия очистки.</span><span class="sxs-lookup"><span data-stu-id="efbac-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="efbac-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="efbac-155">Response</span></span>
<span data-ttu-id="efbac-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсинформатионпротектионвипеактион](../resources/intune-mam-windowsinformationprotectionwipeaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efbac-156">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efbac-157">Пример</span><span class="sxs-lookup"><span data-stu-id="efbac-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="efbac-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="efbac-158">Request</span></span>
<span data-ttu-id="efbac-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efbac-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efbac-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="efbac-160">Response</span></span>
<span data-ttu-id="efbac-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efbac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





