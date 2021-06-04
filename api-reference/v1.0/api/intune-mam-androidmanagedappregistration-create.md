---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b4b2db4b6b725caddf5323450a993aff685af8e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745445"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="b52b3-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="b52b3-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="b52b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b52b3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b52b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b52b3-106">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b52b3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b52b3-107">Prerequisites</span></span>
<span data-ttu-id="b52b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b52b3-110">Permission type</span></span>|<span data-ttu-id="b52b3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b52b3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b52b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b52b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b52b3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52b3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b52b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b52b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b52b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52b3-115">Not supported.</span></span>|
|<span data-ttu-id="b52b3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b52b3-116">Application</span></span>|<span data-ttu-id="b52b3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52b3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b52b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b52b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="b52b3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b52b3-119">Request headers</span></span>
|<span data-ttu-id="b52b3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b52b3-120">Header</span></span>|<span data-ttu-id="b52b3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b52b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b52b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b52b3-122">Authorization</span></span>|<span data-ttu-id="b52b3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b52b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b52b3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b52b3-124">Accept</span></span>|<span data-ttu-id="b52b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b52b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52b3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b52b3-126">Request body</span></span>
<span data-ttu-id="b52b3-127">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b52b3-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="b52b3-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="b52b3-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="b52b3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b52b3-129">Property</span></span>|<span data-ttu-id="b52b3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b52b3-130">Type</span></span>|<span data-ttu-id="b52b3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b52b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b52b3-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b52b3-132">createdDateTime</span></span>|<span data-ttu-id="b52b3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52b3-133">DateTimeOffset</span></span>|<span data-ttu-id="b52b3-134">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b52b3-135">lastSyncDateTime</span></span>|<span data-ttu-id="b52b3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52b3-136">DateTimeOffset</span></span>|<span data-ttu-id="b52b3-137">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="b52b3-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="b52b3-138">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="b52b3-139">applicationVersion</span></span>|<span data-ttu-id="b52b3-140">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-140">String</span></span>|<span data-ttu-id="b52b3-141">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="b52b3-142">managementSdkVersion</span></span>|<span data-ttu-id="b52b3-143">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-143">String</span></span>|<span data-ttu-id="b52b3-144">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="b52b3-145">platformVersion</span></span>|<span data-ttu-id="b52b3-146">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-146">String</span></span>|<span data-ttu-id="b52b3-147">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="b52b3-148">deviceType</span></span>|<span data-ttu-id="b52b3-149">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-149">String</span></span>|<span data-ttu-id="b52b3-150">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b52b3-151">deviceTag</span></span>|<span data-ttu-id="b52b3-152">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-152">String</span></span>|<span data-ttu-id="b52b3-153">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="b52b3-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="b52b3-154">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="b52b3-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="b52b3-155">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="b52b3-156">deviceName</span></span>|<span data-ttu-id="b52b3-157">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-157">String</span></span>|<span data-ttu-id="b52b3-158">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-159">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="b52b3-159">flaggedReasons</span></span>|<span data-ttu-id="b52b3-160">[коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="b52b3-160">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="b52b3-161">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="b52b3-161">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="b52b3-162">(например,</span><span class="sxs-lookup"><span data-stu-id="b52b3-162">E.g.</span></span> <span data-ttu-id="b52b3-163">приложение, запущенное на корневом устройстве, унаследовано от [управляемогоAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-163">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="b52b3-164">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="b52b3-164">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="b52b3-165">userId</span><span class="sxs-lookup"><span data-stu-id="b52b3-165">userId</span></span>|<span data-ttu-id="b52b3-166">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-166">String</span></span>|<span data-ttu-id="b52b3-167">Идентификатор пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="b52b3-167">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="b52b3-168">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-169">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="b52b3-169">appIdentifier</span></span>|[<span data-ttu-id="b52b3-170">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b52b3-170">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b52b3-171">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-171">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-172">id</span><span class="sxs-lookup"><span data-stu-id="b52b3-172">id</span></span>|<span data-ttu-id="b52b3-173">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-173">String</span></span>|<span data-ttu-id="b52b3-174">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b52b3-174">Key of the entity.</span></span> <span data-ttu-id="b52b3-175">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-175">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="b52b3-176">version</span><span class="sxs-lookup"><span data-stu-id="b52b3-176">version</span></span>|<span data-ttu-id="b52b3-177">String</span><span class="sxs-lookup"><span data-stu-id="b52b3-177">String</span></span>|<span data-ttu-id="b52b3-178">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="b52b3-178">Version of the entity.</span></span> <span data-ttu-id="b52b3-179">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b52b3-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b52b3-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52b3-180">Response</span></span>
<span data-ttu-id="b52b3-181">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b52b3-181">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52b3-182">Пример</span><span class="sxs-lookup"><span data-stu-id="b52b3-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="b52b3-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="b52b3-183">Request</span></span>
<span data-ttu-id="b52b3-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b52b3-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b52b3-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52b3-185">Response</span></span>
<span data-ttu-id="b52b3-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b52b3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




