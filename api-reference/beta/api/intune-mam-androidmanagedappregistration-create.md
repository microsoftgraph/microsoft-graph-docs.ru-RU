---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 21215cddf0966a6a209e10609ac5620053daa919
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974205"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="a3416-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a3416-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="a3416-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3416-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3416-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3416-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3416-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3416-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3416-107">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-107">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3416-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3416-108">Prerequisites</span></span>
<span data-ttu-id="a3416-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3416-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3416-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3416-111">Permission type</span></span>|<span data-ttu-id="a3416-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3416-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3416-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3416-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3416-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3416-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a3416-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3416-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3416-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3416-116">Not supported.</span></span>|
|<span data-ttu-id="a3416-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3416-117">Application</span></span>|<span data-ttu-id="a3416-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3416-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3416-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3416-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="a3416-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3416-120">Request headers</span></span>
|<span data-ttu-id="a3416-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3416-121">Header</span></span>|<span data-ttu-id="a3416-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3416-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3416-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3416-123">Authorization</span></span>|<span data-ttu-id="a3416-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3416-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3416-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3416-125">Accept</span></span>|<span data-ttu-id="a3416-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3416-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3416-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3416-127">Request body</span></span>
<span data-ttu-id="a3416-128">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3416-128">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="a3416-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="a3416-129">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="a3416-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3416-130">Property</span></span>|<span data-ttu-id="a3416-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3416-131">Type</span></span>|<span data-ttu-id="a3416-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3416-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3416-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3416-133">createdDateTime</span></span>|<span data-ttu-id="a3416-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3416-134">DateTimeOffset</span></span>|<span data-ttu-id="a3416-135">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-135">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a3416-136">lastSyncDateTime</span></span>|<span data-ttu-id="a3416-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3416-137">DateTimeOffset</span></span>|<span data-ttu-id="a3416-138">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="a3416-138">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="a3416-139">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-139">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-140">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="a3416-140">applicationVersion</span></span>|<span data-ttu-id="a3416-141">String</span><span class="sxs-lookup"><span data-stu-id="a3416-141">String</span></span>|<span data-ttu-id="a3416-142">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-142">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-143">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="a3416-143">managementSdkVersion</span></span>|<span data-ttu-id="a3416-144">String</span><span class="sxs-lookup"><span data-stu-id="a3416-144">String</span></span>|<span data-ttu-id="a3416-145">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-145">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-146">platformVersion</span><span class="sxs-lookup"><span data-stu-id="a3416-146">platformVersion</span></span>|<span data-ttu-id="a3416-147">String</span><span class="sxs-lookup"><span data-stu-id="a3416-147">String</span></span>|<span data-ttu-id="a3416-148">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-148">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-149">deviceType</span><span class="sxs-lookup"><span data-stu-id="a3416-149">deviceType</span></span>|<span data-ttu-id="a3416-150">String</span><span class="sxs-lookup"><span data-stu-id="a3416-150">String</span></span>|<span data-ttu-id="a3416-151">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-151">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-152">deviceTag</span><span class="sxs-lookup"><span data-stu-id="a3416-152">deviceTag</span></span>|<span data-ttu-id="a3416-153">String</span><span class="sxs-lookup"><span data-stu-id="a3416-153">String</span></span>|<span data-ttu-id="a3416-154">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a3416-154">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="a3416-155">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="a3416-155">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="a3416-156">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-156">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-157">deviceName</span><span class="sxs-lookup"><span data-stu-id="a3416-157">deviceName</span></span>|<span data-ttu-id="a3416-158">String</span><span class="sxs-lookup"><span data-stu-id="a3416-158">String</span></span>|<span data-ttu-id="a3416-159">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-159">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a3416-160">managedDeviceId</span></span>|<span data-ttu-id="a3416-161">Строка</span><span class="sxs-lookup"><span data-stu-id="a3416-161">String</span></span>|<span data-ttu-id="a3416-162">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="a3416-162">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="a3416-163">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="a3416-163">Value could be empty even when the host device is managed.</span></span> <span data-ttu-id="a3416-164">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-165">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a3416-165">azureADDeviceId</span></span>|<span data-ttu-id="a3416-166">String</span><span class="sxs-lookup"><span data-stu-id="a3416-166">String</span></span>|<span data-ttu-id="a3416-167">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="a3416-167">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="a3416-168">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="a3416-168">Value could be empty even when the host device is Azure Active Directory registered.</span></span> <span data-ttu-id="a3416-169">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-170">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a3416-170">deviceModel</span></span>|<span data-ttu-id="a3416-171">String</span><span class="sxs-lookup"><span data-stu-id="a3416-171">String</span></span>|<span data-ttu-id="a3416-172">Модель устройства для текущего приложения регистрация Inherited [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a3416-172">The device model for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-173">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="a3416-173">deviceManufacturer</span></span>|<span data-ttu-id="a3416-174">Строка</span><span class="sxs-lookup"><span data-stu-id="a3416-174">String</span></span>|<span data-ttu-id="a3416-175">Производитель устройства для текущего приложения регистрация Inherited [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a3416-175">The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-176">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="a3416-176">flaggedReasons</span></span>|<span data-ttu-id="a3416-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a3416-177">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="a3416-178">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="a3416-178">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="a3416-179">Пример:</span><span class="sxs-lookup"><span data-stu-id="a3416-179">E.g.</span></span> <span data-ttu-id="a3416-180">приложения, работающего на устройстве корневые унаследованные от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-180">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="a3416-181">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="a3416-181">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="a3416-182">userId</span><span class="sxs-lookup"><span data-stu-id="a3416-182">userId</span></span>|<span data-ttu-id="a3416-183">String</span><span class="sxs-lookup"><span data-stu-id="a3416-183">String</span></span>|<span data-ttu-id="a3416-184">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="a3416-184">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="a3416-185">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-186">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="a3416-186">appIdentifier</span></span>|[<span data-ttu-id="a3416-187">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a3416-187">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a3416-188">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-188">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-189">id</span><span class="sxs-lookup"><span data-stu-id="a3416-189">id</span></span>|<span data-ttu-id="a3416-190">Строка</span><span class="sxs-lookup"><span data-stu-id="a3416-190">String</span></span>|<span data-ttu-id="a3416-191">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3416-191">Key of the entity.</span></span> <span data-ttu-id="a3416-192">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-192">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="a3416-193">version</span><span class="sxs-lookup"><span data-stu-id="a3416-193">version</span></span>|<span data-ttu-id="a3416-194">Строка</span><span class="sxs-lookup"><span data-stu-id="a3416-194">String</span></span>|<span data-ttu-id="a3416-195">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a3416-195">Version of the entity.</span></span> <span data-ttu-id="a3416-196">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a3416-196">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a3416-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3416-197">Response</span></span>
<span data-ttu-id="a3416-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a3416-198">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3416-199">Пример</span><span class="sxs-lookup"><span data-stu-id="a3416-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3416-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3416-200">Request</span></span>
<span data-ttu-id="a3416-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3416-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3416-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3416-202">Response</span></span>
<span data-ttu-id="a3416-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3416-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





