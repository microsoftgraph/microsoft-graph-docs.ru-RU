---
title: Создание Андроидманажедстореаппконфигуратион
description: Создание нового объекта Андроидманажедстореаппконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee33f730fa05e1bb7a9640622960a37b926d1780
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986273"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="5f9f7-103">Создание Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5f9f7-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="5f9f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f9f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f9f7-106">Создание нового объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5f9f7-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f9f7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f9f7-107">Prerequisites</span></span>
<span data-ttu-id="5f9f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f9f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f9f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f9f7-110">Permission type</span></span>|<span data-ttu-id="5f9f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f9f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f9f7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f9f7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f9f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f9f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-115">Not supported.</span></span>|
|<span data-ttu-id="5f9f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f9f7-116">Application</span></span>|<span data-ttu-id="5f9f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f9f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f9f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5f9f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f9f7-119">Request headers</span></span>
|<span data-ttu-id="5f9f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f9f7-120">Header</span></span>|<span data-ttu-id="5f9f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5f9f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f9f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f9f7-122">Authorization</span></span>|<span data-ttu-id="5f9f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f9f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f9f7-124">Accept</span></span>|<span data-ttu-id="5f9f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f9f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f9f7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5f9f7-126">Request body</span></span>
<span data-ttu-id="5f9f7-127">В тексте запроса добавьте представление объекта Андроидманажедстореаппконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="5f9f7-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореаппконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="5f9f7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f9f7-129">Property</span></span>|<span data-ttu-id="5f9f7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5f9f7-130">Type</span></span>|<span data-ttu-id="5f9f7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5f9f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f9f7-132">id</span><span class="sxs-lookup"><span data-stu-id="5f9f7-132">id</span></span>|<span data-ttu-id="5f9f7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5f9f7-133">String</span></span>|<span data-ttu-id="5f9f7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-134">Key of the entity.</span></span> <span data-ttu-id="5f9f7-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5f9f7-136">targetedMobileApps</span></span>|<span data-ttu-id="5f9f7-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5f9f7-137">String collection</span></span>|<span data-ttu-id="5f9f7-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="5f9f7-138">the associated app.</span></span> <span data-ttu-id="5f9f7-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5f9f7-140">roleScopeTagIds</span></span>|<span data-ttu-id="5f9f7-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5f9f7-141">String collection</span></span>|<span data-ttu-id="5f9f7-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="5f9f7-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f9f7-144">createdDateTime</span></span>|<span data-ttu-id="5f9f7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f9f7-145">DateTimeOffset</span></span>|<span data-ttu-id="5f9f7-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-146">DateTime the object was created.</span></span> <span data-ttu-id="5f9f7-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-148">description</span><span class="sxs-lookup"><span data-stu-id="5f9f7-148">description</span></span>|<span data-ttu-id="5f9f7-149">String</span><span class="sxs-lookup"><span data-stu-id="5f9f7-149">String</span></span>|<span data-ttu-id="5f9f7-150">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f9f7-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f9f7-152">lastModifiedDateTime</span></span>|<span data-ttu-id="5f9f7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f9f7-153">DateTimeOffset</span></span>|<span data-ttu-id="5f9f7-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-154">DateTime the object was last modified.</span></span> <span data-ttu-id="5f9f7-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5f9f7-156">displayName</span></span>|<span data-ttu-id="5f9f7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="5f9f7-157">String</span></span>|<span data-ttu-id="5f9f7-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f9f7-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-160">версия</span><span class="sxs-lookup"><span data-stu-id="5f9f7-160">version</span></span>|<span data-ttu-id="5f9f7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5f9f7-161">Int32</span></span>|<span data-ttu-id="5f9f7-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-162">Version of the device configuration.</span></span> <span data-ttu-id="5f9f7-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5f9f7-164">packageId</span><span class="sxs-lookup"><span data-stu-id="5f9f7-164">packageId</span></span>|<span data-ttu-id="5f9f7-165">String</span><span class="sxs-lookup"><span data-stu-id="5f9f7-165">String</span></span>|<span data-ttu-id="5f9f7-166">Идентификатор пакета конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="5f9f7-167">Пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="5f9f7-167">payloadJson</span></span>|<span data-ttu-id="5f9f7-168">String</span><span class="sxs-lookup"><span data-stu-id="5f9f7-168">String</span></span>|<span data-ttu-id="5f9f7-169">Полезные данные JSON конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="5f9f7-170">Пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="5f9f7-170">permissionActions</span></span>|<span data-ttu-id="5f9f7-171">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5f9f7-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="5f9f7-172">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="5f9f7-173">Аппсуппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="5f9f7-173">appSupportsOemConfig</span></span>|<span data-ttu-id="5f9f7-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f9f7-174">Boolean</span></span>|<span data-ttu-id="5f9f7-175">Указывает, является ли Аппконфиг политикой Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5f9f7-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f9f7-176">Response</span></span>
<span data-ttu-id="5f9f7-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-177">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f9f7-178">Пример</span><span class="sxs-lookup"><span data-stu-id="5f9f7-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f9f7-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f9f7-179">Request</span></span>
<span data-ttu-id="5f9f7-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 592

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "appSupportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="5f9f7-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f9f7-181">Response</span></span>
<span data-ttu-id="5f9f7-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f9f7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 764

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "919a9335-9335-919a-3593-9a9135939a91",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "appSupportsOemConfig": true
}
```




