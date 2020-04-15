---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d62f07d8daa7b6c4244d4f8feef6a48102eb74d8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446048"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="1dbfa-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1dbfa-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="1dbfa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dbfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dbfa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dbfa-106">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dbfa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1dbfa-107">Prerequisites</span></span>
<span data-ttu-id="1dbfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dbfa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dbfa-110">Permission type</span></span>|<span data-ttu-id="1dbfa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dbfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dbfa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dbfa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dbfa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbfa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1dbfa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dbfa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dbfa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-115">Not supported.</span></span>|
|<span data-ttu-id="1dbfa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dbfa-116">Application</span></span>|<span data-ttu-id="1dbfa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dbfa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dbfa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="1dbfa-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1dbfa-119">Request headers</span></span>
|<span data-ttu-id="1dbfa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dbfa-120">Header</span></span>|<span data-ttu-id="1dbfa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1dbfa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dbfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dbfa-122">Authorization</span></span>|<span data-ttu-id="1dbfa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dbfa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1dbfa-124">Accept</span></span>|<span data-ttu-id="1dbfa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1dbfa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbfa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1dbfa-126">Request body</span></span>
<span data-ttu-id="1dbfa-127">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="1dbfa-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="1dbfa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dbfa-129">Property</span></span>|<span data-ttu-id="1dbfa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1dbfa-130">Type</span></span>|<span data-ttu-id="1dbfa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1dbfa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbfa-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dbfa-132">createdDateTime</span></span>|<span data-ttu-id="1dbfa-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dbfa-133">DateTimeOffset</span></span>|<span data-ttu-id="1dbfa-134">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1dbfa-135">lastSyncDateTime</span></span>|<span data-ttu-id="1dbfa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dbfa-136">DateTimeOffset</span></span>|<span data-ttu-id="1dbfa-137">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="1dbfa-138">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="1dbfa-139">applicationVersion</span></span>|<span data-ttu-id="1dbfa-140">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-140">String</span></span>|<span data-ttu-id="1dbfa-141">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="1dbfa-142">managementSdkVersion</span></span>|<span data-ttu-id="1dbfa-143">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-143">String</span></span>|<span data-ttu-id="1dbfa-144">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="1dbfa-145">platformVersion</span></span>|<span data-ttu-id="1dbfa-146">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-146">String</span></span>|<span data-ttu-id="1dbfa-147">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="1dbfa-148">deviceType</span></span>|<span data-ttu-id="1dbfa-149">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-149">String</span></span>|<span data-ttu-id="1dbfa-150">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1dbfa-151">deviceTag</span></span>|<span data-ttu-id="1dbfa-152">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-152">String</span></span>|<span data-ttu-id="1dbfa-153">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="1dbfa-154">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="1dbfa-155">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="1dbfa-156">deviceName</span></span>|<span data-ttu-id="1dbfa-157">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-157">String</span></span>|<span data-ttu-id="1dbfa-158">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-159">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="1dbfa-159">flaggedReasons</span></span>|<span data-ttu-id="1dbfa-160">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="1dbfa-160">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="1dbfa-161">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="1dbfa-161">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="1dbfa-162">(например,</span><span class="sxs-lookup"><span data-stu-id="1dbfa-162">E.g.</span></span> <span data-ttu-id="1dbfa-163">приложение, работающее на корневом устройстве, унаследованном от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-163">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="1dbfa-164">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-164">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="1dbfa-165">userId</span><span class="sxs-lookup"><span data-stu-id="1dbfa-165">userId</span></span>|<span data-ttu-id="1dbfa-166">String</span><span class="sxs-lookup"><span data-stu-id="1dbfa-166">String</span></span>|<span data-ttu-id="1dbfa-167">Идентификатор пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-167">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="1dbfa-168">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-169">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="1dbfa-169">appIdentifier</span></span>|[<span data-ttu-id="1dbfa-170">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1dbfa-170">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="1dbfa-171">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-171">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-172">id</span><span class="sxs-lookup"><span data-stu-id="1dbfa-172">id</span></span>|<span data-ttu-id="1dbfa-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1dbfa-173">String</span></span>|<span data-ttu-id="1dbfa-174">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-174">Key of the entity.</span></span> <span data-ttu-id="1dbfa-175">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-175">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="1dbfa-176">version</span><span class="sxs-lookup"><span data-stu-id="1dbfa-176">version</span></span>|<span data-ttu-id="1dbfa-177">Строка</span><span class="sxs-lookup"><span data-stu-id="1dbfa-177">String</span></span>|<span data-ttu-id="1dbfa-178">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-178">Version of the entity.</span></span> <span data-ttu-id="1dbfa-179">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbfa-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1dbfa-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbfa-180">Response</span></span>
<span data-ttu-id="1dbfa-181">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-181">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dbfa-182">Пример</span><span class="sxs-lookup"><span data-stu-id="1dbfa-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dbfa-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dbfa-183">Request</span></span>
<span data-ttu-id="1dbfa-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dbfa-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbfa-185">Response</span></span>
<span data-ttu-id="1dbfa-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dbfa-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






