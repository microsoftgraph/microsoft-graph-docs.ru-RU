---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3c0b4901db4ee277b4f2470bc62aaffd00bbea3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145532"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="54877-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="54877-103">Create androidManagedAppRegistration</span></span>

<span data-ttu-id="54877-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54877-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54877-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54877-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54877-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54877-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54877-107">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54877-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="54877-108">Prerequisites</span></span>
<span data-ttu-id="54877-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54877-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54877-111">Permission type</span></span>|<span data-ttu-id="54877-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54877-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54877-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54877-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54877-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54877-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54877-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54877-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54877-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54877-116">Not supported.</span></span>|
|<span data-ttu-id="54877-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="54877-117">Application</span></span>|<span data-ttu-id="54877-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54877-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54877-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54877-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="54877-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="54877-120">Request headers</span></span>
|<span data-ttu-id="54877-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54877-121">Header</span></span>|<span data-ttu-id="54877-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54877-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54877-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54877-123">Authorization</span></span>|<span data-ttu-id="54877-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54877-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54877-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54877-125">Accept</span></span>|<span data-ttu-id="54877-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54877-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54877-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54877-127">Request body</span></span>
<span data-ttu-id="54877-128">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54877-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="54877-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="54877-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="54877-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54877-130">Property</span></span>|<span data-ttu-id="54877-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54877-131">Type</span></span>|<span data-ttu-id="54877-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54877-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54877-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54877-133">createdDateTime</span></span>|<span data-ttu-id="54877-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54877-134">DateTimeOffset</span></span>|<span data-ttu-id="54877-135">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="54877-136">lastSyncDateTime</span></span>|<span data-ttu-id="54877-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54877-137">DateTimeOffset</span></span>|<span data-ttu-id="54877-138">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="54877-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="54877-139">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="54877-140">applicationVersion</span></span>|<span data-ttu-id="54877-141">String</span><span class="sxs-lookup"><span data-stu-id="54877-141">String</span></span>|<span data-ttu-id="54877-142">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="54877-143">managementSdkVersion</span></span>|<span data-ttu-id="54877-144">String</span><span class="sxs-lookup"><span data-stu-id="54877-144">String</span></span>|<span data-ttu-id="54877-145">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="54877-146">platformVersion</span></span>|<span data-ttu-id="54877-147">String</span><span class="sxs-lookup"><span data-stu-id="54877-147">String</span></span>|<span data-ttu-id="54877-148">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="54877-149">deviceType</span></span>|<span data-ttu-id="54877-150">String</span><span class="sxs-lookup"><span data-stu-id="54877-150">String</span></span>|<span data-ttu-id="54877-151">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="54877-152">deviceTag</span></span>|<span data-ttu-id="54877-153">String</span><span class="sxs-lookup"><span data-stu-id="54877-153">String</span></span>|<span data-ttu-id="54877-154">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="54877-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="54877-155">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="54877-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="54877-156">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="54877-157">deviceName</span></span>|<span data-ttu-id="54877-158">String</span><span class="sxs-lookup"><span data-stu-id="54877-158">String</span></span>|<span data-ttu-id="54877-159">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="54877-160">managedDeviceId</span></span>|<span data-ttu-id="54877-161">Строка</span><span class="sxs-lookup"><span data-stu-id="54877-161">String</span></span>|<span data-ttu-id="54877-162">Идентификатор управляемого устройства хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="54877-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="54877-163">Значение может быть пустым даже при управляемом устройстве хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="54877-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="54877-164">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="54877-165">azureADDeviceId</span></span>|<span data-ttu-id="54877-166">String</span><span class="sxs-lookup"><span data-stu-id="54877-166">String</span></span>|<span data-ttu-id="54877-167">Идентификатор устройства Azure Active Directory для хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="54877-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="54877-168">Значение может быть пустым даже при регистрации устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="54877-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="54877-169">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="54877-170">deviceModel</span></span>|<span data-ttu-id="54877-171">String</span><span class="sxs-lookup"><span data-stu-id="54877-171">String</span></span>|<span data-ttu-id="54877-172">Модель устройства для текущей регистрации приложений, унаследованной от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="54877-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="54877-173">deviceManufacturer</span></span>|<span data-ttu-id="54877-174">Строка</span><span class="sxs-lookup"><span data-stu-id="54877-174">String</span></span>|<span data-ttu-id="54877-175">Производитель устройств для текущей регистрации приложений, унаследованных от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="54877-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="54877-176">flaggedReasons</span></span>|<span data-ttu-id="54877-177">[коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="54877-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="54877-178">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="54877-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="54877-179">(например,</span><span class="sxs-lookup"><span data-stu-id="54877-179">E.g.</span></span> <span data-ttu-id="54877-180">приложение, запущенное на корневом устройстве, унаследовано от [управляемогоAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="54877-181">Возможные значения: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span><span class="sxs-lookup"><span data-stu-id="54877-181">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="54877-182">userId</span><span class="sxs-lookup"><span data-stu-id="54877-182">userId</span></span>|<span data-ttu-id="54877-183">String</span><span class="sxs-lookup"><span data-stu-id="54877-183">String</span></span>|<span data-ttu-id="54877-184">Идентификатор пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="54877-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="54877-185">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="54877-186">appIdentifier</span></span>|[<span data-ttu-id="54877-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="54877-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="54877-188">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-189">id</span><span class="sxs-lookup"><span data-stu-id="54877-189">id</span></span>|<span data-ttu-id="54877-190">Строка</span><span class="sxs-lookup"><span data-stu-id="54877-190">String</span></span>|<span data-ttu-id="54877-191">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54877-191">Key of the entity.</span></span> <span data-ttu-id="54877-192">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-193">version</span><span class="sxs-lookup"><span data-stu-id="54877-193">version</span></span>|<span data-ttu-id="54877-194">String</span><span class="sxs-lookup"><span data-stu-id="54877-194">String</span></span>|<span data-ttu-id="54877-195">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="54877-195">Version of the entity.</span></span> <span data-ttu-id="54877-196">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="54877-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="54877-197">patchVersion</span><span class="sxs-lookup"><span data-stu-id="54877-197">patchVersion</span></span>|<span data-ttu-id="54877-198">Строка</span><span class="sxs-lookup"><span data-stu-id="54877-198">String</span></span>|<span data-ttu-id="54877-199">Версия патча для текущей регистрации android-приложений</span><span class="sxs-lookup"><span data-stu-id="54877-199">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="54877-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="54877-200">Response</span></span>
<span data-ttu-id="54877-201">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="54877-201">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54877-202">Пример</span><span class="sxs-lookup"><span data-stu-id="54877-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="54877-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="54877-203">Request</span></span>
<span data-ttu-id="54877-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54877-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="54877-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="54877-205">Response</span></span>
<span data-ttu-id="54877-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54877-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

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
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```




