---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 83a2fd4c1967da5bdb401ab57bf603dace128f05
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408497"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="f4f31-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f4f31-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="f4f31-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f4f31-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4f31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4f31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4f31-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4f31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f31-107">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f31-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4f31-108">Prerequisites</span></span>
<span data-ttu-id="f4f31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4f31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4f31-111">Permission type</span></span>|<span data-ttu-id="f4f31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4f31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4f31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4f31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4f31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4f31-116">Not supported.</span></span>|
|<span data-ttu-id="f4f31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4f31-117">Application</span></span>|<span data-ttu-id="f4f31-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4f31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4f31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="f4f31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4f31-120">Request headers</span></span>
|<span data-ttu-id="f4f31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4f31-121">Header</span></span>|<span data-ttu-id="f4f31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4f31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4f31-123">Authorization</span></span>|<span data-ttu-id="f4f31-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4f31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4f31-125">Accept</span></span>|<span data-ttu-id="f4f31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f31-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4f31-127">Request body</span></span>
<span data-ttu-id="f4f31-128">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4f31-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="f4f31-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="f4f31-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="f4f31-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4f31-130">Property</span></span>|<span data-ttu-id="f4f31-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f4f31-131">Type</span></span>|<span data-ttu-id="f4f31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f4f31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f31-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4f31-133">createdDateTime</span></span>|<span data-ttu-id="f4f31-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4f31-134">DateTimeOffset</span></span>|<span data-ttu-id="f4f31-135">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f4f31-136">lastSyncDateTime</span></span>|<span data-ttu-id="f4f31-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4f31-137">DateTimeOffset</span></span>|<span data-ttu-id="f4f31-138">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="f4f31-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="f4f31-139">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="f4f31-140">applicationVersion</span></span>|<span data-ttu-id="f4f31-141">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-141">String</span></span>|<span data-ttu-id="f4f31-142">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f4f31-143">managementSdkVersion</span></span>|<span data-ttu-id="f4f31-144">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-144">String</span></span>|<span data-ttu-id="f4f31-145">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="f4f31-146">platformVersion</span></span>|<span data-ttu-id="f4f31-147">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-147">String</span></span>|<span data-ttu-id="f4f31-148">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="f4f31-149">deviceType</span></span>|<span data-ttu-id="f4f31-150">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-150">String</span></span>|<span data-ttu-id="f4f31-151">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f4f31-152">deviceTag</span></span>|<span data-ttu-id="f4f31-153">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-153">String</span></span>|<span data-ttu-id="f4f31-154">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f4f31-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="f4f31-155">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="f4f31-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="f4f31-156">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="f4f31-157">deviceName</span></span>|<span data-ttu-id="f4f31-158">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-158">String</span></span>|<span data-ttu-id="f4f31-159">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f4f31-160">managedDeviceId</span></span>|<span data-ttu-id="f4f31-161">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-161">String</span></span>|<span data-ttu-id="f4f31-162">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="f4f31-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="f4f31-163">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="f4f31-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="f4f31-164">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f4f31-165">azureADDeviceId</span></span>|<span data-ttu-id="f4f31-166">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-166">String</span></span>|<span data-ttu-id="f4f31-167">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="f4f31-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="f4f31-168">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="f4f31-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="f4f31-169">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f4f31-170">deviceModel</span></span>|<span data-ttu-id="f4f31-171">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-171">String</span></span>|<span data-ttu-id="f4f31-172">Модель устройства для текущего приложения регистрация Inherited [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="f4f31-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="f4f31-173">deviceManufacturer</span></span>|<span data-ttu-id="f4f31-174">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-174">String</span></span>|<span data-ttu-id="f4f31-175">Производитель устройства для текущего приложения регистрация Inherited [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="f4f31-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="f4f31-176">flaggedReasons</span></span>|<span data-ttu-id="f4f31-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f4f31-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="f4f31-178">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="f4f31-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="f4f31-179">Пример:</span><span class="sxs-lookup"><span data-stu-id="f4f31-179">E.g.</span></span> <span data-ttu-id="f4f31-180">приложения, работающего на устройстве корневые унаследованные от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="f4f31-181">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="f4f31-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="f4f31-182">userId</span><span class="sxs-lookup"><span data-stu-id="f4f31-182">userId</span></span>|<span data-ttu-id="f4f31-183">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-183">String</span></span>|<span data-ttu-id="f4f31-184">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="f4f31-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="f4f31-185">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4f31-186">appIdentifier</span></span>|[<span data-ttu-id="f4f31-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4f31-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f4f31-188">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-189">id</span><span class="sxs-lookup"><span data-stu-id="f4f31-189">id</span></span>|<span data-ttu-id="f4f31-190">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-190">String</span></span>|<span data-ttu-id="f4f31-191">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4f31-191">Key of the entity.</span></span> <span data-ttu-id="f4f31-192">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-193">version</span><span class="sxs-lookup"><span data-stu-id="f4f31-193">version</span></span>|<span data-ttu-id="f4f31-194">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-194">String</span></span>|<span data-ttu-id="f4f31-195">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="f4f31-195">Version of the entity.</span></span> <span data-ttu-id="f4f31-196">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f4f31-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="f4f31-197">patchVersion</span><span class="sxs-lookup"><span data-stu-id="f4f31-197">patchVersion</span></span>|<span data-ttu-id="f4f31-198">String</span><span class="sxs-lookup"><span data-stu-id="f4f31-198">String</span></span>|<span data-ttu-id="f4f31-199">Версия исправления для текущей регистрации приложения для android</span><span class="sxs-lookup"><span data-stu-id="f4f31-199">The patch version for the current android app registration</span></span>|



## <a name="response"></a><span data-ttu-id="f4f31-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4f31-200">Response</span></span>
<span data-ttu-id="f4f31-201">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4f31-201">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f31-202">Пример</span><span class="sxs-lookup"><span data-stu-id="f4f31-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4f31-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4f31-203">Request</span></span>
<span data-ttu-id="f4f31-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4f31-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4f31-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4f31-205">Response</span></span>
<span data-ttu-id="f4f31-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f4f31-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




