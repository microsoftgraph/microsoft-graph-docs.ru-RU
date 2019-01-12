---
title: Создание androidForWorkMobileAppConfiguration
description: Создание нового объекта androidForWorkMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c512d35d8f37ed19b132641742942ca3c47aad2b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990617"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="ad884-103">Создание androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad884-103">Create androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="ad884-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad884-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad884-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad884-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad884-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad884-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad884-107">Создание нового объекта [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ad884-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad884-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad884-108">Prerequisites</span></span>
<span data-ttu-id="ad884-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad884-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad884-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad884-111">Permission type</span></span>|<span data-ttu-id="ad884-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad884-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad884-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad884-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad884-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad884-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad884-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad884-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad884-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad884-116">Not supported.</span></span>|
|<span data-ttu-id="ad884-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad884-117">Application</span></span>|<span data-ttu-id="ad884-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad884-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad884-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad884-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ad884-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad884-120">Request headers</span></span>
|<span data-ttu-id="ad884-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad884-121">Header</span></span>|<span data-ttu-id="ad884-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad884-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad884-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad884-123">Authorization</span></span>|<span data-ttu-id="ad884-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad884-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad884-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad884-125">Accept</span></span>|<span data-ttu-id="ad884-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad884-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad884-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad884-127">Request body</span></span>
<span data-ttu-id="ad884-128">В тексте запроса укажите представление JSON для объекта androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad884-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="ad884-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad884-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="ad884-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad884-130">Property</span></span>|<span data-ttu-id="ad884-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad884-131">Type</span></span>|<span data-ttu-id="ad884-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad884-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad884-133">id</span><span class="sxs-lookup"><span data-stu-id="ad884-133">id</span></span>|<span data-ttu-id="ad884-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ad884-134">String</span></span>|<span data-ttu-id="ad884-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ad884-135">Key of the entity.</span></span> <span data-ttu-id="ad884-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ad884-137">targetedMobileApps</span></span>|<span data-ttu-id="ad884-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad884-138">String collection</span></span>|<span data-ttu-id="ad884-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="ad884-139">the associated app.</span></span> <span data-ttu-id="ad884-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad884-141">roleScopeTagIds</span></span>|<span data-ttu-id="ad884-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad884-142">String collection</span></span>|<span data-ttu-id="ad884-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="ad884-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="ad884-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad884-145">createdDateTime</span></span>|<span data-ttu-id="ad884-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad884-146">DateTimeOffset</span></span>|<span data-ttu-id="ad884-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ad884-147">DateTime the object was created.</span></span> <span data-ttu-id="ad884-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-149">описание</span><span class="sxs-lookup"><span data-stu-id="ad884-149">description</span></span>|<span data-ttu-id="ad884-150">Строка</span><span class="sxs-lookup"><span data-stu-id="ad884-150">String</span></span>|<span data-ttu-id="ad884-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="ad884-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad884-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad884-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ad884-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad884-154">DateTimeOffset</span></span>|<span data-ttu-id="ad884-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ad884-155">DateTime the object was last modified.</span></span> <span data-ttu-id="ad884-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-157">displayName</span><span class="sxs-lookup"><span data-stu-id="ad884-157">displayName</span></span>|<span data-ttu-id="ad884-158">Строка</span><span class="sxs-lookup"><span data-stu-id="ad884-158">String</span></span>|<span data-ttu-id="ad884-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad884-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad884-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-161">версия</span><span class="sxs-lookup"><span data-stu-id="ad884-161">version</span></span>|<span data-ttu-id="ad884-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ad884-162">Int32</span></span>|<span data-ttu-id="ad884-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad884-163">Version of the device configuration.</span></span> <span data-ttu-id="ad884-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="ad884-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ad884-165">packageId</span><span class="sxs-lookup"><span data-stu-id="ad884-165">packageId</span></span>|<span data-ttu-id="ad884-166">String</span><span class="sxs-lookup"><span data-stu-id="ad884-166">String</span></span>|<span data-ttu-id="ad884-167">Идентификатор пакета конфигурации Android для работы приложения.</span><span class="sxs-lookup"><span data-stu-id="ad884-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="ad884-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="ad884-168">payloadJson</span></span>|<span data-ttu-id="ad884-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ad884-169">String</span></span>|<span data-ttu-id="ad884-170">Полезной нагрузки JSON конфигурации приложения Android для работы.</span><span class="sxs-lookup"><span data-stu-id="ad884-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="ad884-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="ad884-171">permissionActions</span></span>|<span data-ttu-id="ad884-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ad884-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="ad884-173">Список разрешений для Android и соответствующие действия разрешений.</span><span class="sxs-lookup"><span data-stu-id="ad884-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="ad884-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad884-174">Response</span></span>
<span data-ttu-id="ad884-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad884-175">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad884-176">Пример</span><span class="sxs-lookup"><span data-stu-id="ad884-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad884-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad884-177">Request</span></span>
<span data-ttu-id="ad884-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad884-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad884-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad884-179">Response</span></span>
<span data-ttu-id="ad884-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad884-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





