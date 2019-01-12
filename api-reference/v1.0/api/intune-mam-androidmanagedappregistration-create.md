---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4485ab59a2a1bc4658a12e9bff4fae57fae2c898
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931995"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="6c4bf-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6c4bf-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="6c4bf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c4bf-105">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c4bf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6c4bf-106">Prerequisites</span></span>
<span data-ttu-id="6c4bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c4bf-109">Permission type</span></span>|<span data-ttu-id="6c4bf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c4bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c4bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c4bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c4bf-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c4bf-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c4bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c4bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c4bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-114">Not supported.</span></span>|
|<span data-ttu-id="6c4bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c4bf-115">Application</span></span>|<span data-ttu-id="6c4bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c4bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c4bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="6c4bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c4bf-118">Request headers</span></span>
|<span data-ttu-id="6c4bf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c4bf-119">Header</span></span>|<span data-ttu-id="6c4bf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6c4bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c4bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c4bf-121">Authorization</span></span>|<span data-ttu-id="6c4bf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6c4bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c4bf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6c4bf-123">Accept</span></span>|<span data-ttu-id="6c4bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c4bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c4bf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c4bf-125">Request body</span></span>
<span data-ttu-id="6c4bf-126">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="6c4bf-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="6c4bf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c4bf-128">Property</span></span>|<span data-ttu-id="6c4bf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6c4bf-129">Type</span></span>|<span data-ttu-id="6c4bf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6c4bf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c4bf-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c4bf-131">createdDateTime</span></span>|<span data-ttu-id="6c4bf-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4bf-132">DateTimeOffset</span></span>|<span data-ttu-id="6c4bf-133">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6c4bf-134">lastSyncDateTime</span></span>|<span data-ttu-id="6c4bf-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4bf-135">DateTimeOffset</span></span>|<span data-ttu-id="6c4bf-136">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="6c4bf-137">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="6c4bf-138">applicationVersion</span></span>|<span data-ttu-id="6c4bf-139">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-139">String</span></span>|<span data-ttu-id="6c4bf-140">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6c4bf-141">managementSdkVersion</span></span>|<span data-ttu-id="6c4bf-142">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-142">String</span></span>|<span data-ttu-id="6c4bf-143">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="6c4bf-144">platformVersion</span></span>|<span data-ttu-id="6c4bf-145">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-145">String</span></span>|<span data-ttu-id="6c4bf-146">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="6c4bf-147">deviceType</span></span>|<span data-ttu-id="6c4bf-148">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-148">String</span></span>|<span data-ttu-id="6c4bf-149">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="6c4bf-150">deviceTag</span></span>|<span data-ttu-id="6c4bf-151">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-151">String</span></span>|<span data-ttu-id="6c4bf-152">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="6c4bf-153">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="6c4bf-154">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="6c4bf-155">deviceName</span></span>|<span data-ttu-id="6c4bf-156">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-156">String</span></span>|<span data-ttu-id="6c4bf-157">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="6c4bf-158">flaggedReasons</span></span>|<span data-ttu-id="6c4bf-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6c4bf-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="6c4bf-160">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="6c4bf-161">Пример:</span><span class="sxs-lookup"><span data-stu-id="6c4bf-161">E.g.</span></span> <span data-ttu-id="6c4bf-162">приложения, работающего на устройстве корневые унаследованные от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="6c4bf-163">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="6c4bf-164">userId</span><span class="sxs-lookup"><span data-stu-id="6c4bf-164">userId</span></span>|<span data-ttu-id="6c4bf-165">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-165">String</span></span>|<span data-ttu-id="6c4bf-166">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="6c4bf-167">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6c4bf-168">appIdentifier</span></span>|[<span data-ttu-id="6c4bf-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6c4bf-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6c4bf-170">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-171">id</span><span class="sxs-lookup"><span data-stu-id="6c4bf-171">id</span></span>|<span data-ttu-id="6c4bf-172">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-172">String</span></span>|<span data-ttu-id="6c4bf-173">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-173">Key of the entity.</span></span> <span data-ttu-id="6c4bf-174">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="6c4bf-175">version</span><span class="sxs-lookup"><span data-stu-id="6c4bf-175">version</span></span>|<span data-ttu-id="6c4bf-176">String</span><span class="sxs-lookup"><span data-stu-id="6c4bf-176">String</span></span>|<span data-ttu-id="6c4bf-177">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-177">Version of the entity.</span></span> <span data-ttu-id="6c4bf-178">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4bf-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6c4bf-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4bf-179">Response</span></span>
<span data-ttu-id="6c4bf-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c4bf-181">Пример</span><span class="sxs-lookup"><span data-stu-id="6c4bf-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c4bf-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c4bf-182">Request</span></span>
<span data-ttu-id="6c4bf-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="6c4bf-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4bf-184">Response</span></span>
<span data-ttu-id="6c4bf-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6c4bf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



