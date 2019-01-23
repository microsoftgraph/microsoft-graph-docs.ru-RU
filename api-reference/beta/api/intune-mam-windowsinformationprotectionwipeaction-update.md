---
title: Обновление windowsInformationProtectionWipeAction
description: Обновление свойства объекта windowsInformationProtectionWipeAction.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49b79d6ebd12d81332613c646623d68dc0b09a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430738"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="c7dc5-103">Обновление windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="c7dc5-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="c7dc5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7dc5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7dc5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7dc5-107">Обновление свойства объекта [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="c7dc5-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7dc5-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c7dc5-108">Prerequisites</span></span>
<span data-ttu-id="c7dc5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7dc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7dc5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7dc5-111">Permission type</span></span>|<span data-ttu-id="c7dc5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7dc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7dc5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7dc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7dc5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7dc5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7dc5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7dc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7dc5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-116">Not supported.</span></span>|
|<span data-ttu-id="c7dc5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7dc5-117">Application</span></span>|<span data-ttu-id="c7dc5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7dc5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7dc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="c7dc5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7dc5-120">Request headers</span></span>
|<span data-ttu-id="c7dc5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7dc5-121">Header</span></span>|<span data-ttu-id="c7dc5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7dc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7dc5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7dc5-123">Authorization</span></span>|<span data-ttu-id="c7dc5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7dc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7dc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7dc5-125">Accept</span></span>|<span data-ttu-id="c7dc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7dc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7dc5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7dc5-127">Request body</span></span>
<span data-ttu-id="c7dc5-128">В тексте запроса укажите представление JSON для объекта [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="c7dc5-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="c7dc5-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="c7dc5-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="c7dc5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7dc5-130">Property</span></span>|<span data-ttu-id="c7dc5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7dc5-131">Type</span></span>|<span data-ttu-id="c7dc5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7dc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7dc5-133">id</span><span class="sxs-lookup"><span data-stu-id="c7dc5-133">id</span></span>|<span data-ttu-id="c7dc5-134">String</span><span class="sxs-lookup"><span data-stu-id="c7dc5-134">String</span></span>|<span data-ttu-id="c7dc5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-135">Key of the entity.</span></span>|
|<span data-ttu-id="c7dc5-136">status</span><span class="sxs-lookup"><span data-stu-id="c7dc5-136">status</span></span>|[<span data-ttu-id="c7dc5-137">actionState</span><span class="sxs-lookup"><span data-stu-id="c7dc5-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c7dc5-138">Очистка состояние действия.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-138">Wipe action status.</span></span> <span data-ttu-id="c7dc5-139">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c7dc5-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="c7dc5-140">targetedUserId</span></span>|<span data-ttu-id="c7dc5-141">String</span><span class="sxs-lookup"><span data-stu-id="c7dc5-141">String</span></span>|<span data-ttu-id="c7dc5-142">Идентификатор пользователя, с это действие очистки.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="c7dc5-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c7dc5-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="c7dc5-144">String</span><span class="sxs-lookup"><span data-stu-id="c7dc5-144">String</span></span>|<span data-ttu-id="c7dc5-145">DeviceRegistrationId с этой операции очистки.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="c7dc5-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c7dc5-146">targetedDeviceName</span></span>|<span data-ttu-id="c7dc5-147">String</span><span class="sxs-lookup"><span data-stu-id="c7dc5-147">String</span></span>|<span data-ttu-id="c7dc5-148">Имя целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-148">Targeted device name.</span></span>|
|<span data-ttu-id="c7dc5-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="c7dc5-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="c7dc5-150">String</span><span class="sxs-lookup"><span data-stu-id="c7dc5-150">String</span></span>|<span data-ttu-id="c7dc5-151">Целевые устройства Mac-адрес.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-151">Targeted device Mac address.</span></span>|



## <a name="response"></a><span data-ttu-id="c7dc5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7dc5-152">Response</span></span>
<span data-ttu-id="c7dc5-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-153">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7dc5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c7dc5-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7dc5-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7dc5-155">Request</span></span>
<span data-ttu-id="c7dc5-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```

### <a name="response"></a><span data-ttu-id="c7dc5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7dc5-157">Response</span></span>
<span data-ttu-id="c7dc5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7dc5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```




