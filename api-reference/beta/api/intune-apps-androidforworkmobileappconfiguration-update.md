---
title: Обновление androidForWorkMobileAppConfiguration
description: Обновление свойства объекта androidForWorkMobileAppConfiguration.
author: tfitzmac
ms.openlocfilehash: 4e9874ef1becc3840320e85872451a8573b95f53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320211"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="3bd40-103">Обновление androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bd40-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="3bd40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3bd40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bd40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bd40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bd40-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3bd40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bd40-107">Обновление свойства объекта [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3bd40-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bd40-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3bd40-108">Prerequisites</span></span>
<span data-ttu-id="3bd40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bd40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bd40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bd40-111">Permission type</span></span>|<span data-ttu-id="3bd40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bd40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bd40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bd40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bd40-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd40-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bd40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bd40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bd40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bd40-116">Not supported.</span></span>|
|<span data-ttu-id="3bd40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bd40-117">Application</span></span>|<span data-ttu-id="3bd40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bd40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bd40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bd40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3bd40-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bd40-120">Request headers</span></span>
|<span data-ttu-id="3bd40-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bd40-121">Header</span></span>|<span data-ttu-id="3bd40-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3bd40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bd40-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bd40-123">Authorization</span></span>|<span data-ttu-id="3bd40-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3bd40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bd40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3bd40-125">Accept</span></span>|<span data-ttu-id="3bd40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bd40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bd40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bd40-127">Request body</span></span>
<span data-ttu-id="3bd40-128">В тексте запроса укажите представление JSON для объекта [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3bd40-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="3bd40-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bd40-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="3bd40-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bd40-130">Property</span></span>|<span data-ttu-id="3bd40-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3bd40-131">Type</span></span>|<span data-ttu-id="3bd40-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3bd40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bd40-133">id</span><span class="sxs-lookup"><span data-stu-id="3bd40-133">id</span></span>|<span data-ttu-id="3bd40-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3bd40-134">String</span></span>|<span data-ttu-id="3bd40-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3bd40-135">Key of the entity.</span></span> <span data-ttu-id="3bd40-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3bd40-137">targetedMobileApps</span></span>|<span data-ttu-id="3bd40-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3bd40-138">String collection</span></span>|<span data-ttu-id="3bd40-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="3bd40-139">the associated app.</span></span> <span data-ttu-id="3bd40-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3bd40-141">roleScopeTagIds</span></span>|<span data-ttu-id="3bd40-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3bd40-142">String collection</span></span>|<span data-ttu-id="3bd40-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="3bd40-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="3bd40-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bd40-145">createdDateTime</span></span>|<span data-ttu-id="3bd40-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bd40-146">DateTimeOffset</span></span>|<span data-ttu-id="3bd40-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3bd40-147">DateTime the object was created.</span></span> <span data-ttu-id="3bd40-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-149">описание</span><span class="sxs-lookup"><span data-stu-id="3bd40-149">description</span></span>|<span data-ttu-id="3bd40-150">Строка</span><span class="sxs-lookup"><span data-stu-id="3bd40-150">String</span></span>|<span data-ttu-id="3bd40-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="3bd40-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3bd40-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bd40-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3bd40-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bd40-154">DateTimeOffset</span></span>|<span data-ttu-id="3bd40-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3bd40-155">DateTime the object was last modified.</span></span> <span data-ttu-id="3bd40-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-157">displayName</span><span class="sxs-lookup"><span data-stu-id="3bd40-157">displayName</span></span>|<span data-ttu-id="3bd40-158">Строка</span><span class="sxs-lookup"><span data-stu-id="3bd40-158">String</span></span>|<span data-ttu-id="3bd40-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bd40-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3bd40-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-161">версия</span><span class="sxs-lookup"><span data-stu-id="3bd40-161">version</span></span>|<span data-ttu-id="3bd40-162">Int32</span><span class="sxs-lookup"><span data-stu-id="3bd40-162">Int32</span></span>|<span data-ttu-id="3bd40-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bd40-163">Version of the device configuration.</span></span> <span data-ttu-id="3bd40-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bd40-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bd40-165">packageId</span><span class="sxs-lookup"><span data-stu-id="3bd40-165">packageId</span></span>|<span data-ttu-id="3bd40-166">String</span><span class="sxs-lookup"><span data-stu-id="3bd40-166">String</span></span>|<span data-ttu-id="3bd40-167">Идентификатор пакета конфигурации Android для работы приложения.</span><span class="sxs-lookup"><span data-stu-id="3bd40-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="3bd40-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="3bd40-168">payloadJson</span></span>|<span data-ttu-id="3bd40-169">String.</span><span class="sxs-lookup"><span data-stu-id="3bd40-169">String</span></span>|<span data-ttu-id="3bd40-170">Полезной нагрузки JSON конфигурации приложения Android для работы.</span><span class="sxs-lookup"><span data-stu-id="3bd40-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="3bd40-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="3bd40-171">permissionActions</span></span>|<span data-ttu-id="3bd40-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3bd40-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="3bd40-173">Список разрешений для Android и соответствующие действия разрешений.</span><span class="sxs-lookup"><span data-stu-id="3bd40-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="3bd40-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bd40-174">Response</span></span>
<span data-ttu-id="3bd40-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3bd40-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bd40-176">Пример</span><span class="sxs-lookup"><span data-stu-id="3bd40-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bd40-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bd40-177">Request</span></span>
<span data-ttu-id="3bd40-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bd40-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 549

{
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

### <a name="response"></a><span data-ttu-id="3bd40-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bd40-179">Response</span></span>
<span data-ttu-id="3bd40-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3bd40-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 732

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
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





