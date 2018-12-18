---
title: Создание androidManagedStoreAppConfiguration
description: Создание нового объекта androidManagedStoreAppConfiguration.
author: tfitzmac
ms.openlocfilehash: 1eb403a9547808969694b4e3712d4b2bcd1995f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361070"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="c6680-103">Создание androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6680-103">Create androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="c6680-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6680-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6680-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6680-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6680-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c6680-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6680-107">Создание нового объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c6680-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6680-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c6680-108">Prerequisites</span></span>
<span data-ttu-id="c6680-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6680-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6680-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6680-111">Permission type</span></span>|<span data-ttu-id="c6680-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6680-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6680-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6680-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6680-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6680-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6680-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6680-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6680-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6680-116">Not supported.</span></span>|
|<span data-ttu-id="c6680-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6680-117">Application</span></span>|<span data-ttu-id="c6680-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6680-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6680-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6680-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c6680-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6680-120">Request headers</span></span>
|<span data-ttu-id="c6680-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6680-121">Header</span></span>|<span data-ttu-id="c6680-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c6680-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6680-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6680-123">Authorization</span></span>|<span data-ttu-id="c6680-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c6680-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6680-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6680-125">Accept</span></span>|<span data-ttu-id="c6680-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6680-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6680-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6680-127">Request body</span></span>
<span data-ttu-id="c6680-128">В тексте запроса укажите представление JSON для объекта androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c6680-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="c6680-129">В следующей таблице показаны свойства, которые необходимы для создания androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c6680-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="c6680-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6680-130">Property</span></span>|<span data-ttu-id="c6680-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c6680-131">Type</span></span>|<span data-ttu-id="c6680-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c6680-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6680-133">id</span><span class="sxs-lookup"><span data-stu-id="c6680-133">id</span></span>|<span data-ttu-id="c6680-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c6680-134">String</span></span>|<span data-ttu-id="c6680-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c6680-135">Key of the entity.</span></span> <span data-ttu-id="c6680-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c6680-137">targetedMobileApps</span></span>|<span data-ttu-id="c6680-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c6680-138">String collection</span></span>|<span data-ttu-id="c6680-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="c6680-139">the associated app.</span></span> <span data-ttu-id="c6680-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c6680-141">roleScopeTagIds</span></span>|<span data-ttu-id="c6680-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c6680-142">String collection</span></span>|<span data-ttu-id="c6680-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="c6680-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="c6680-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6680-145">createdDateTime</span></span>|<span data-ttu-id="c6680-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6680-146">DateTimeOffset</span></span>|<span data-ttu-id="c6680-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c6680-147">DateTime the object was created.</span></span> <span data-ttu-id="c6680-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-149">описание</span><span class="sxs-lookup"><span data-stu-id="c6680-149">description</span></span>|<span data-ttu-id="c6680-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c6680-150">String</span></span>|<span data-ttu-id="c6680-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="c6680-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c6680-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6680-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c6680-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6680-154">DateTimeOffset</span></span>|<span data-ttu-id="c6680-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c6680-155">DateTime the object was last modified.</span></span> <span data-ttu-id="c6680-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-157">displayName</span><span class="sxs-lookup"><span data-stu-id="c6680-157">displayName</span></span>|<span data-ttu-id="c6680-158">Строка</span><span class="sxs-lookup"><span data-stu-id="c6680-158">String</span></span>|<span data-ttu-id="c6680-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c6680-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c6680-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-161">версия</span><span class="sxs-lookup"><span data-stu-id="c6680-161">version</span></span>|<span data-ttu-id="c6680-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c6680-162">Int32</span></span>|<span data-ttu-id="c6680-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c6680-163">Version of the device configuration.</span></span> <span data-ttu-id="c6680-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c6680-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c6680-165">packageId</span><span class="sxs-lookup"><span data-stu-id="c6680-165">packageId</span></span>|<span data-ttu-id="c6680-166">String</span><span class="sxs-lookup"><span data-stu-id="c6680-166">String</span></span>|<span data-ttu-id="c6680-167">Идентификатор приложения пакета конфигурации Android предприятия.</span><span class="sxs-lookup"><span data-stu-id="c6680-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="c6680-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="c6680-168">payloadJson</span></span>|<span data-ttu-id="c6680-169">String.</span><span class="sxs-lookup"><span data-stu-id="c6680-169">String</span></span>|<span data-ttu-id="c6680-170">Android корпоративного приложения конфигурации JSON полезных данных.</span><span class="sxs-lookup"><span data-stu-id="c6680-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="c6680-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="c6680-171">permissionActions</span></span>|<span data-ttu-id="c6680-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c6680-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="c6680-173">Список разрешений для Android и соответствующие действия разрешений.</span><span class="sxs-lookup"><span data-stu-id="c6680-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="c6680-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6680-174">Response</span></span>
<span data-ttu-id="c6680-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c6680-175">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6680-176">Пример</span><span class="sxs-lookup"><span data-stu-id="c6680-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6680-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6680-177">Request</span></span>
<span data-ttu-id="c6680-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6680-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 623

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="c6680-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6680-179">Response</span></span>
<span data-ttu-id="c6680-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c6680-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 731

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
  ]
}
```





