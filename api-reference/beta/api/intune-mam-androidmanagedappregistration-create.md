---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9460cba5969f601ec656aeee0899892311e38e59
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193420"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="e2214-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e2214-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="e2214-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2214-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2214-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2214-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2214-106">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-106">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2214-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e2214-107">Prerequisites</span></span>
<span data-ttu-id="e2214-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2214-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2214-110">Permission type</span></span>|<span data-ttu-id="e2214-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2214-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2214-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2214-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2214-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2214-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2214-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2214-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2214-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2214-115">Not supported.</span></span>|
|<span data-ttu-id="e2214-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2214-116">Application</span></span>|<span data-ttu-id="e2214-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2214-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2214-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2214-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="e2214-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2214-119">Request headers</span></span>
|<span data-ttu-id="e2214-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2214-120">Header</span></span>|<span data-ttu-id="e2214-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e2214-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2214-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2214-122">Authorization</span></span>|<span data-ttu-id="e2214-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2214-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2214-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e2214-124">Accept</span></span>|<span data-ttu-id="e2214-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2214-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2214-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2214-126">Request body</span></span>
<span data-ttu-id="e2214-127">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2214-127">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="e2214-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="e2214-128">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="e2214-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2214-129">Property</span></span>|<span data-ttu-id="e2214-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e2214-130">Type</span></span>|<span data-ttu-id="e2214-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e2214-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2214-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2214-132">createdDateTime</span></span>|<span data-ttu-id="e2214-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2214-133">DateTimeOffset</span></span>|<span data-ttu-id="e2214-134">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-134">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e2214-135">lastSyncDateTime</span></span>|<span data-ttu-id="e2214-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2214-136">DateTimeOffset</span></span>|<span data-ttu-id="e2214-137">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="e2214-137">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="e2214-138">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-138">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-139">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="e2214-139">applicationVersion</span></span>|<span data-ttu-id="e2214-140">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-140">String</span></span>|<span data-ttu-id="e2214-141">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-141">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-142">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="e2214-142">managementSdkVersion</span></span>|<span data-ttu-id="e2214-143">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-143">String</span></span>|<span data-ttu-id="e2214-144">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-144">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-145">platformVersion</span><span class="sxs-lookup"><span data-stu-id="e2214-145">platformVersion</span></span>|<span data-ttu-id="e2214-146">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-146">String</span></span>|<span data-ttu-id="e2214-147">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-147">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-148">deviceType</span><span class="sxs-lookup"><span data-stu-id="e2214-148">deviceType</span></span>|<span data-ttu-id="e2214-149">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-149">String</span></span>|<span data-ttu-id="e2214-150">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-150">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-151">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e2214-151">deviceTag</span></span>|<span data-ttu-id="e2214-152">String</span><span class="sxs-lookup"><span data-stu-id="e2214-152">String</span></span>|<span data-ttu-id="e2214-153">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e2214-153">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="e2214-154">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="e2214-154">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="e2214-155">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-155">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="e2214-156">deviceName</span></span>|<span data-ttu-id="e2214-157">String</span><span class="sxs-lookup"><span data-stu-id="e2214-157">String</span></span>|<span data-ttu-id="e2214-158">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-158">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-159">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="e2214-159">managedDeviceId</span></span>|<span data-ttu-id="e2214-160">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-160">String</span></span>|<span data-ttu-id="e2214-161">Управляемый идентификатор устройства хоста.</span><span class="sxs-lookup"><span data-stu-id="e2214-161">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="e2214-162">Значение может быть пустым, даже если ведущее устройство управляется.</span><span class="sxs-lookup"><span data-stu-id="e2214-162">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="e2214-163">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-163">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-164">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="e2214-164">azureADDeviceId</span></span>|<span data-ttu-id="e2214-165">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-165">String</span></span>|<span data-ttu-id="e2214-166">Идентификатор устройства Azure Active Directory ведущего устройства.</span><span class="sxs-lookup"><span data-stu-id="e2214-166">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="e2214-167">Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e2214-167">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="e2214-168">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-169">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e2214-169">deviceModel</span></span>|<span data-ttu-id="e2214-170">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-170">String</span></span>|<span data-ttu-id="e2214-171">Модель устройства для текущей регистрации приложения наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="e2214-171">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-172">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="e2214-172">deviceManufacturer</span></span>|<span data-ttu-id="e2214-173">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-173">String</span></span>|<span data-ttu-id="e2214-174">Производитель устройства для текущей регистрации приложения, унаследованный от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="e2214-174">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-175">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="e2214-175">flaggedReasons</span></span>|<span data-ttu-id="e2214-176">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="e2214-176">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="e2214-177">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e2214-177">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="e2214-178">(например,</span><span class="sxs-lookup"><span data-stu-id="e2214-178">E.g.</span></span> <span data-ttu-id="e2214-179">приложение, работающее на корневом устройстве, унаследованном от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-179">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="e2214-180">Возможные значения: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span><span class="sxs-lookup"><span data-stu-id="e2214-180">Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.</span></span>|
|<span data-ttu-id="e2214-181">userId</span><span class="sxs-lookup"><span data-stu-id="e2214-181">userId</span></span>|<span data-ttu-id="e2214-182">String</span><span class="sxs-lookup"><span data-stu-id="e2214-182">String</span></span>|<span data-ttu-id="e2214-183">Идентификатор пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="e2214-183">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="e2214-184">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-185">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2214-185">appIdentifier</span></span>|[<span data-ttu-id="e2214-186">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2214-186">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e2214-187">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-187">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-188">id</span><span class="sxs-lookup"><span data-stu-id="e2214-188">id</span></span>|<span data-ttu-id="e2214-189">Строка</span><span class="sxs-lookup"><span data-stu-id="e2214-189">String</span></span>|<span data-ttu-id="e2214-190">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2214-190">Key of the entity.</span></span> <span data-ttu-id="e2214-191">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-191">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-192">version</span><span class="sxs-lookup"><span data-stu-id="e2214-192">version</span></span>|<span data-ttu-id="e2214-193">Строка</span><span class="sxs-lookup"><span data-stu-id="e2214-193">String</span></span>|<span data-ttu-id="e2214-194">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e2214-194">Version of the entity.</span></span> <span data-ttu-id="e2214-195">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e2214-195">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="e2214-196">патчверсион</span><span class="sxs-lookup"><span data-stu-id="e2214-196">patchVersion</span></span>|<span data-ttu-id="e2214-197">String.</span><span class="sxs-lookup"><span data-stu-id="e2214-197">String</span></span>|<span data-ttu-id="e2214-198">Версия исправления для текущей регистрации приложений Android</span><span class="sxs-lookup"><span data-stu-id="e2214-198">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="e2214-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2214-199">Response</span></span>
<span data-ttu-id="e2214-200">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2214-200">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2214-201">Пример</span><span class="sxs-lookup"><span data-stu-id="e2214-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2214-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2214-202">Request</span></span>
<span data-ttu-id="e2214-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2214-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2214-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2214-204">Response</span></span>
<span data-ttu-id="e2214-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2214-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




