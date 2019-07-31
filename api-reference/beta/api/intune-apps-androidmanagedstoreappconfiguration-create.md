---
title: Создание Андроидманажедстореаппконфигуратион
description: Создание нового объекта Андроидманажедстореаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af0a0d02b7877c17c1211af4b7e8e01b208ea1f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952179"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="7220a-103">Создание Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7220a-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="7220a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7220a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7220a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7220a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7220a-106">Создание нового объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7220a-106">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7220a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7220a-107">Prerequisites</span></span>
<span data-ttu-id="7220a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7220a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7220a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7220a-110">Permission type</span></span>|<span data-ttu-id="7220a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7220a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7220a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7220a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7220a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7220a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7220a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7220a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7220a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7220a-115">Not supported.</span></span>|
|<span data-ttu-id="7220a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7220a-116">Application</span></span>|<span data-ttu-id="7220a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7220a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7220a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7220a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7220a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7220a-119">Request headers</span></span>
|<span data-ttu-id="7220a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7220a-120">Header</span></span>|<span data-ttu-id="7220a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7220a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7220a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7220a-122">Authorization</span></span>|<span data-ttu-id="7220a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7220a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7220a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7220a-124">Accept</span></span>|<span data-ttu-id="7220a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7220a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7220a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7220a-126">Request body</span></span>
<span data-ttu-id="7220a-127">В тексте запроса добавьте представление объекта Андроидманажедстореаппконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7220a-127">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="7220a-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореаппконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="7220a-128">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="7220a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7220a-129">Property</span></span>|<span data-ttu-id="7220a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7220a-130">Type</span></span>|<span data-ttu-id="7220a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7220a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7220a-132">id</span><span class="sxs-lookup"><span data-stu-id="7220a-132">id</span></span>|<span data-ttu-id="7220a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7220a-133">String</span></span>|<span data-ttu-id="7220a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7220a-134">Key of the entity.</span></span> <span data-ttu-id="7220a-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7220a-136">targetedMobileApps</span></span>|<span data-ttu-id="7220a-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7220a-137">String collection</span></span>|<span data-ttu-id="7220a-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="7220a-138">the associated app.</span></span> <span data-ttu-id="7220a-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7220a-140">roleScopeTagIds</span></span>|<span data-ttu-id="7220a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7220a-141">String collection</span></span>|<span data-ttu-id="7220a-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7220a-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="7220a-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7220a-144">createdDateTime</span></span>|<span data-ttu-id="7220a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7220a-145">DateTimeOffset</span></span>|<span data-ttu-id="7220a-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7220a-146">DateTime the object was created.</span></span> <span data-ttu-id="7220a-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-148">description</span><span class="sxs-lookup"><span data-stu-id="7220a-148">description</span></span>|<span data-ttu-id="7220a-149">String</span><span class="sxs-lookup"><span data-stu-id="7220a-149">String</span></span>|<span data-ttu-id="7220a-150">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7220a-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7220a-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7220a-152">lastModifiedDateTime</span></span>|<span data-ttu-id="7220a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7220a-153">DateTimeOffset</span></span>|<span data-ttu-id="7220a-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7220a-154">DateTime the object was last modified.</span></span> <span data-ttu-id="7220a-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-156">displayName</span><span class="sxs-lookup"><span data-stu-id="7220a-156">displayName</span></span>|<span data-ttu-id="7220a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="7220a-157">String</span></span>|<span data-ttu-id="7220a-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7220a-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7220a-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-160">версия</span><span class="sxs-lookup"><span data-stu-id="7220a-160">version</span></span>|<span data-ttu-id="7220a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="7220a-161">Int32</span></span>|<span data-ttu-id="7220a-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7220a-162">Version of the device configuration.</span></span> <span data-ttu-id="7220a-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7220a-164">packageId</span><span class="sxs-lookup"><span data-stu-id="7220a-164">packageId</span></span>|<span data-ttu-id="7220a-165">String</span><span class="sxs-lookup"><span data-stu-id="7220a-165">String</span></span>|<span data-ttu-id="7220a-166">Идентификатор пакета конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="7220a-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="7220a-167">Пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="7220a-167">payloadJson</span></span>|<span data-ttu-id="7220a-168">String</span><span class="sxs-lookup"><span data-stu-id="7220a-168">String</span></span>|<span data-ttu-id="7220a-169">Полезные данные JSON конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="7220a-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="7220a-170">Пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="7220a-170">permissionActions</span></span>|<span data-ttu-id="7220a-171">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="7220a-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="7220a-172">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="7220a-172">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="7220a-173">Аппсуппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="7220a-173">appSupportsOemConfig</span></span>|<span data-ttu-id="7220a-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="7220a-174">Boolean</span></span>|<span data-ttu-id="7220a-175">Указывает, является ли Аппконфиг политикой Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="7220a-175">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="7220a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="7220a-176">Response</span></span>
<span data-ttu-id="7220a-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7220a-177">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7220a-178">Пример</span><span class="sxs-lookup"><span data-stu-id="7220a-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="7220a-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="7220a-179">Request</span></span>
<span data-ttu-id="7220a-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7220a-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7220a-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="7220a-181">Response</span></span>
<span data-ttu-id="7220a-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7220a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





