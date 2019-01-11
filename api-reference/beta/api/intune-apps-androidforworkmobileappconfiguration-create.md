---
title: Создание androidForWorkMobileAppConfiguration
description: Создание нового объекта androidForWorkMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 013c4856bc40614b49108715b0d66b4af8f93890
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844416"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="7b0e2-103">Создание androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b0e2-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="7b0e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b0e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b0e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b0e2-107">Создание нового объекта [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7b0e2-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b0e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b0e2-108">Prerequisites</span></span>
<span data-ttu-id="7b0e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b0e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b0e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b0e2-111">Permission type</span></span>|<span data-ttu-id="7b0e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b0e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b0e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b0e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b0e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b0e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7b0e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b0e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b0e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-116">Not supported.</span></span>|
|<span data-ttu-id="7b0e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b0e2-117">Application</span></span>|<span data-ttu-id="7b0e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b0e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b0e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b0e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b0e2-120">Request headers</span></span>
|<span data-ttu-id="7b0e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b0e2-121">Header</span></span>|<span data-ttu-id="7b0e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b0e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b0e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b0e2-123">Authorization</span></span>|<span data-ttu-id="7b0e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7b0e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b0e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b0e2-125">Accept</span></span>|<span data-ttu-id="7b0e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b0e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b0e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b0e2-127">Request body</span></span>
<span data-ttu-id="7b0e2-128">В тексте запроса укажите представление JSON для объекта androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="7b0e2-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="7b0e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b0e2-130">Property</span></span>|<span data-ttu-id="7b0e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b0e2-131">Type</span></span>|<span data-ttu-id="7b0e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b0e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b0e2-133">id</span><span class="sxs-lookup"><span data-stu-id="7b0e2-133">id</span></span>|<span data-ttu-id="7b0e2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7b0e2-134">String</span></span>|<span data-ttu-id="7b0e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-135">Key of the entity.</span></span> <span data-ttu-id="7b0e2-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7b0e2-137">targetedMobileApps</span></span>|<span data-ttu-id="7b0e2-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7b0e2-138">String collection</span></span>|<span data-ttu-id="7b0e2-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="7b0e2-139">the associated app.</span></span> <span data-ttu-id="7b0e2-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b0e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="7b0e2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7b0e2-142">String collection</span></span>|<span data-ttu-id="7b0e2-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="7b0e2-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b0e2-145">createdDateTime</span></span>|<span data-ttu-id="7b0e2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b0e2-146">DateTimeOffset</span></span>|<span data-ttu-id="7b0e2-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-147">DateTime the object was created.</span></span> <span data-ttu-id="7b0e2-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-149">описание</span><span class="sxs-lookup"><span data-stu-id="7b0e2-149">description</span></span>|<span data-ttu-id="7b0e2-150">Строка</span><span class="sxs-lookup"><span data-stu-id="7b0e2-150">String</span></span>|<span data-ttu-id="7b0e2-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b0e2-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b0e2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7b0e2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b0e2-154">DateTimeOffset</span></span>|<span data-ttu-id="7b0e2-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-155">DateTime the object was last modified.</span></span> <span data-ttu-id="7b0e2-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-157">displayName</span><span class="sxs-lookup"><span data-stu-id="7b0e2-157">displayName</span></span>|<span data-ttu-id="7b0e2-158">Строка</span><span class="sxs-lookup"><span data-stu-id="7b0e2-158">String</span></span>|<span data-ttu-id="7b0e2-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b0e2-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-161">версия</span><span class="sxs-lookup"><span data-stu-id="7b0e2-161">version</span></span>|<span data-ttu-id="7b0e2-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7b0e2-162">Int32</span></span>|<span data-ttu-id="7b0e2-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-163">Version of the device configuration.</span></span> <span data-ttu-id="7b0e2-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="7b0e2-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="7b0e2-165">packageId</span><span class="sxs-lookup"><span data-stu-id="7b0e2-165">packageId</span></span>|<span data-ttu-id="7b0e2-166">String</span><span class="sxs-lookup"><span data-stu-id="7b0e2-166">String</span></span>|<span data-ttu-id="7b0e2-167">Идентификатор пакета конфигурации Android для работы приложения.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="7b0e2-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="7b0e2-168">payloadJson</span></span>|<span data-ttu-id="7b0e2-169">Строка</span><span class="sxs-lookup"><span data-stu-id="7b0e2-169">String</span></span>|<span data-ttu-id="7b0e2-170">Полезной нагрузки JSON конфигурации приложения Android для работы.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="7b0e2-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="7b0e2-171">permissionActions</span></span>|<span data-ttu-id="7b0e2-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7b0e2-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="7b0e2-173">Список разрешений для Android и соответствующие действия разрешений.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="7b0e2-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b0e2-174">Response</span></span>
<span data-ttu-id="7b0e2-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-175">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b0e2-176">Пример</span><span class="sxs-lookup"><span data-stu-id="7b0e2-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b0e2-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b0e2-177">Request</span></span>
<span data-ttu-id="7b0e2-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 624

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="7b0e2-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b0e2-179">Response</span></span>
<span data-ttu-id="7b0e2-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b0e2-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





