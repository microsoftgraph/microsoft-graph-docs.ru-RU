---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: c05c698179f2f8fa54ab12282be6e397b9275408
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339510"
---
# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="21542-103">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="21542-103">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="21542-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21542-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21542-105">Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-105">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21542-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21542-106">Prerequisites</span></span>
<span data-ttu-id="21542-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21542-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21542-109">Permission type</span></span>|<span data-ttu-id="21542-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21542-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21542-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21542-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21542-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21542-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21542-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21542-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21542-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21542-114">Not supported.</span></span>|
|<span data-ttu-id="21542-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21542-115">Application</span></span>|<span data-ttu-id="21542-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21542-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21542-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21542-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="21542-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21542-118">Request headers</span></span>
|<span data-ttu-id="21542-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21542-119">Header</span></span>|<span data-ttu-id="21542-120">Значение</span><span class="sxs-lookup"><span data-stu-id="21542-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21542-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21542-121">Authorization</span></span>|<span data-ttu-id="21542-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21542-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21542-123">Accept</span><span class="sxs-lookup"><span data-stu-id="21542-123">Accept</span></span>|<span data-ttu-id="21542-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21542-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21542-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21542-125">Request body</span></span>
<span data-ttu-id="21542-126">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21542-126">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="21542-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="21542-127">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="21542-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="21542-128">Property</span></span>|<span data-ttu-id="21542-129">Тип</span><span class="sxs-lookup"><span data-stu-id="21542-129">Type</span></span>|<span data-ttu-id="21542-130">Описание</span><span class="sxs-lookup"><span data-stu-id="21542-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21542-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21542-131">createdDateTime</span></span>|<span data-ttu-id="21542-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21542-132">DateTimeOffset</span></span>|<span data-ttu-id="21542-133">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-133">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="21542-134">lastSyncDateTime</span></span>|<span data-ttu-id="21542-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21542-135">DateTimeOffset</span></span>|<span data-ttu-id="21542-136">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="21542-136">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="21542-137">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-137">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-138">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="21542-138">applicationVersion</span></span>|<span data-ttu-id="21542-139">String</span><span class="sxs-lookup"><span data-stu-id="21542-139">String</span></span>|<span data-ttu-id="21542-140">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-140">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-141">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="21542-141">managementSdkVersion</span></span>|<span data-ttu-id="21542-142">String</span><span class="sxs-lookup"><span data-stu-id="21542-142">String</span></span>|<span data-ttu-id="21542-143">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-143">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-144">platformVersion</span><span class="sxs-lookup"><span data-stu-id="21542-144">platformVersion</span></span>|<span data-ttu-id="21542-145">String</span><span class="sxs-lookup"><span data-stu-id="21542-145">String</span></span>|<span data-ttu-id="21542-146">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-146">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-147">deviceType</span><span class="sxs-lookup"><span data-stu-id="21542-147">deviceType</span></span>|<span data-ttu-id="21542-148">String</span><span class="sxs-lookup"><span data-stu-id="21542-148">String</span></span>|<span data-ttu-id="21542-149">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-149">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-150">deviceTag</span><span class="sxs-lookup"><span data-stu-id="21542-150">deviceTag</span></span>|<span data-ttu-id="21542-151">String</span><span class="sxs-lookup"><span data-stu-id="21542-151">String</span></span>|<span data-ttu-id="21542-152">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="21542-152">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="21542-153">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="21542-153">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="21542-154">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-154">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="21542-155">deviceName</span></span>|<span data-ttu-id="21542-156">String</span><span class="sxs-lookup"><span data-stu-id="21542-156">String</span></span>|<span data-ttu-id="21542-157">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-157">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-158">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="21542-158">flaggedReasons</span></span>|<span data-ttu-id="21542-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="21542-159">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="21542-160">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="21542-160">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="21542-161">Пример:</span><span class="sxs-lookup"><span data-stu-id="21542-161">E.g.</span></span> <span data-ttu-id="21542-162">приложения, работающего на устройстве корневые унаследованные от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-162">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span></span> <span data-ttu-id="21542-163">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="21542-163">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="21542-164">userId</span><span class="sxs-lookup"><span data-stu-id="21542-164">userId</span></span>|<span data-ttu-id="21542-165">String</span><span class="sxs-lookup"><span data-stu-id="21542-165">String</span></span>|<span data-ttu-id="21542-166">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="21542-166">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="21542-167">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-168">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="21542-168">appIdentifier</span></span>|[<span data-ttu-id="21542-169">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="21542-169">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="21542-170">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-170">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-171">id</span><span class="sxs-lookup"><span data-stu-id="21542-171">id</span></span>|<span data-ttu-id="21542-172">Строка</span><span class="sxs-lookup"><span data-stu-id="21542-172">String</span></span>|<span data-ttu-id="21542-173">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21542-173">Key of the entity.</span></span> <span data-ttu-id="21542-174">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-174">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="21542-175">version</span><span class="sxs-lookup"><span data-stu-id="21542-175">version</span></span>|<span data-ttu-id="21542-176">Строка</span><span class="sxs-lookup"><span data-stu-id="21542-176">String</span></span>|<span data-ttu-id="21542-177">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="21542-177">Version of the entity.</span></span> <span data-ttu-id="21542-178">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="21542-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="21542-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="21542-179">Response</span></span>
<span data-ttu-id="21542-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21542-180">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21542-181">Пример</span><span class="sxs-lookup"><span data-stu-id="21542-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="21542-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="21542-182">Request</span></span>
<span data-ttu-id="21542-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21542-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21542-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="21542-184">Response</span></span>
<span data-ttu-id="21542-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21542-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



