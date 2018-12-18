---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: 074d8d01a086956af1f88e0d0315ccc84b84c9cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326763"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="dab5d-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="dab5d-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="dab5d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dab5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dab5d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dab5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dab5d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dab5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dab5d-107">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dab5d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dab5d-108">Prerequisites</span></span>
<span data-ttu-id="dab5d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dab5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab5d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dab5d-111">Permission type</span></span>|<span data-ttu-id="dab5d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dab5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dab5d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dab5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dab5d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab5d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dab5d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dab5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dab5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dab5d-116">Not supported.</span></span>|
|<span data-ttu-id="dab5d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dab5d-117">Application</span></span>|<span data-ttu-id="dab5d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dab5d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dab5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dab5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="dab5d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dab5d-120">Request headers</span></span>
|<span data-ttu-id="dab5d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dab5d-121">Header</span></span>|<span data-ttu-id="dab5d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dab5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dab5d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dab5d-123">Authorization</span></span>|<span data-ttu-id="dab5d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dab5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dab5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dab5d-125">Accept</span></span>|<span data-ttu-id="dab5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dab5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dab5d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dab5d-127">Request body</span></span>
<span data-ttu-id="dab5d-128">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dab5d-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="dab5d-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="dab5d-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="dab5d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dab5d-130">Property</span></span>|<span data-ttu-id="dab5d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dab5d-131">Type</span></span>|<span data-ttu-id="dab5d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dab5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dab5d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dab5d-133">createdDateTime</span></span>|<span data-ttu-id="dab5d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dab5d-134">DateTimeOffset</span></span>|<span data-ttu-id="dab5d-135">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dab5d-136">lastSyncDateTime</span></span>|<span data-ttu-id="dab5d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dab5d-137">DateTimeOffset</span></span>|<span data-ttu-id="dab5d-138">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="dab5d-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="dab5d-139">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="dab5d-140">applicationVersion</span></span>|<span data-ttu-id="dab5d-141">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-141">String</span></span>|<span data-ttu-id="dab5d-142">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="dab5d-143">managementSdkVersion</span></span>|<span data-ttu-id="dab5d-144">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-144">String</span></span>|<span data-ttu-id="dab5d-145">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="dab5d-146">platformVersion</span></span>|<span data-ttu-id="dab5d-147">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-147">String</span></span>|<span data-ttu-id="dab5d-148">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="dab5d-149">deviceType</span></span>|<span data-ttu-id="dab5d-150">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-150">String</span></span>|<span data-ttu-id="dab5d-151">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="dab5d-152">deviceTag</span></span>|<span data-ttu-id="dab5d-153">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-153">String</span></span>|<span data-ttu-id="dab5d-154">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="dab5d-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="dab5d-155">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="dab5d-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="dab5d-156">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="dab5d-157">deviceName</span></span>|<span data-ttu-id="dab5d-158">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-158">String</span></span>|<span data-ttu-id="dab5d-159">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="dab5d-160">managedDeviceId</span></span>|<span data-ttu-id="dab5d-161">String.</span><span class="sxs-lookup"><span data-stu-id="dab5d-161">String</span></span>|<span data-ttu-id="dab5d-162">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="dab5d-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="dab5d-163">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="dab5d-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="dab5d-164">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="dab5d-165">azureADDeviceId</span></span>|<span data-ttu-id="dab5d-166">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-166">String</span></span>|<span data-ttu-id="dab5d-167">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="dab5d-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="dab5d-168">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="dab5d-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="dab5d-169">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="dab5d-170">deviceModel</span></span>|<span data-ttu-id="dab5d-171">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-171">String</span></span>|<span data-ttu-id="dab5d-172">Модель устройства для текущего приложения регистрация Inherited [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="dab5d-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="dab5d-173">deviceManufacturer</span></span>|<span data-ttu-id="dab5d-174">String.</span><span class="sxs-lookup"><span data-stu-id="dab5d-174">String</span></span>|<span data-ttu-id="dab5d-175">Производитель устройства для текущего приложения регистрация Inherited [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="dab5d-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="dab5d-176">flaggedReasons</span></span>|<span data-ttu-id="dab5d-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="dab5d-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="dab5d-178">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="dab5d-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="dab5d-179">Пример:</span><span class="sxs-lookup"><span data-stu-id="dab5d-179">E.g.</span></span> <span data-ttu-id="dab5d-180">приложения, работающего на устройстве корневые унаследованные от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="dab5d-181">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="dab5d-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="dab5d-182">userId</span><span class="sxs-lookup"><span data-stu-id="dab5d-182">userId</span></span>|<span data-ttu-id="dab5d-183">String</span><span class="sxs-lookup"><span data-stu-id="dab5d-183">String</span></span>|<span data-ttu-id="dab5d-184">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="dab5d-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="dab5d-185">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="dab5d-186">appIdentifier</span></span>|[<span data-ttu-id="dab5d-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="dab5d-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="dab5d-188">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-189">id</span><span class="sxs-lookup"><span data-stu-id="dab5d-189">id</span></span>|<span data-ttu-id="dab5d-190">Строка</span><span class="sxs-lookup"><span data-stu-id="dab5d-190">String</span></span>|<span data-ttu-id="dab5d-191">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dab5d-191">Key of the entity.</span></span> <span data-ttu-id="dab5d-192">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="dab5d-193">version</span><span class="sxs-lookup"><span data-stu-id="dab5d-193">version</span></span>|<span data-ttu-id="dab5d-194">Строка</span><span class="sxs-lookup"><span data-stu-id="dab5d-194">String</span></span>|<span data-ttu-id="dab5d-195">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="dab5d-195">Version of the entity.</span></span> <span data-ttu-id="dab5d-196">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="dab5d-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="dab5d-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="dab5d-197">Response</span></span>
<span data-ttu-id="dab5d-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dab5d-198">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dab5d-199">Пример</span><span class="sxs-lookup"><span data-stu-id="dab5d-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="dab5d-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="dab5d-200">Request</span></span>
<span data-ttu-id="dab5d-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dab5d-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 837

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
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="dab5d-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="dab5d-202">Response</span></span>
<span data-ttu-id="dab5d-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dab5d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 945

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
  "version": "Version value"
}
```





