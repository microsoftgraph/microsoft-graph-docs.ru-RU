---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67c8cb5281d029416e5a5ccc7726565195de3cd2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800608"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="baa7c-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="baa7c-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="baa7c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baa7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baa7c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="baa7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baa7c-106">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baa7c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="baa7c-107">Prerequisites</span></span>
<span data-ttu-id="baa7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baa7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baa7c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baa7c-110">Permission type</span></span>|<span data-ttu-id="baa7c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="baa7c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baa7c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baa7c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="baa7c-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="baa7c-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="baa7c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa7c-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="baa7c-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="baa7c-115">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="baa7c-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa7c-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="baa7c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baa7c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baa7c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baa7c-118">Not supported.</span></span>|
|<span data-ttu-id="baa7c-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="baa7c-119">Application</span></span>||
| <span data-ttu-id="baa7c-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="baa7c-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="baa7c-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa7c-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="baa7c-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="baa7c-122">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="baa7c-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa7c-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="baa7c-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baa7c-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="baa7c-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="baa7c-125">Request headers</span></span>
|<span data-ttu-id="baa7c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="baa7c-126">Header</span></span>|<span data-ttu-id="baa7c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="baa7c-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baa7c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="baa7c-128">Authorization</span></span>|<span data-ttu-id="baa7c-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baa7c-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baa7c-130">Accept</span><span class="sxs-lookup"><span data-stu-id="baa7c-130">Accept</span></span>|<span data-ttu-id="baa7c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="baa7c-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baa7c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="baa7c-132">Request body</span></span>
<span data-ttu-id="baa7c-133">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baa7c-133">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="baa7c-134">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-134">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="baa7c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="baa7c-135">Property</span></span>|<span data-ttu-id="baa7c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="baa7c-136">Type</span></span>|<span data-ttu-id="baa7c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="baa7c-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa7c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="baa7c-138">displayName</span></span>|<span data-ttu-id="baa7c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="baa7c-139">String</span></span>|<span data-ttu-id="baa7c-140">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="baa7c-140">Policy display name.</span></span> <span data-ttu-id="baa7c-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-142">description</span><span class="sxs-lookup"><span data-stu-id="baa7c-142">description</span></span>|<span data-ttu-id="baa7c-143">String</span><span class="sxs-lookup"><span data-stu-id="baa7c-143">String</span></span>|<span data-ttu-id="baa7c-144">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="baa7c-144">The policy's description.</span></span> <span data-ttu-id="baa7c-145">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="baa7c-146">createdDateTime</span></span>|<span data-ttu-id="baa7c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baa7c-147">DateTimeOffset</span></span>|<span data-ttu-id="baa7c-148">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="baa7c-148">The date and time the policy was created.</span></span> <span data-ttu-id="baa7c-149">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baa7c-150">lastModifiedDateTime</span></span>|<span data-ttu-id="baa7c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baa7c-151">DateTimeOffset</span></span>|<span data-ttu-id="baa7c-152">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="baa7c-152">Last time the policy was modified.</span></span> <span data-ttu-id="baa7c-153">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="baa7c-154">roleScopeTagIds</span></span>|<span data-ttu-id="baa7c-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="baa7c-155">String collection</span></span>|<span data-ttu-id="baa7c-156">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="baa7c-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="baa7c-157">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-158">id</span><span class="sxs-lookup"><span data-stu-id="baa7c-158">id</span></span>|<span data-ttu-id="baa7c-159">String</span><span class="sxs-lookup"><span data-stu-id="baa7c-159">String</span></span>|<span data-ttu-id="baa7c-160">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="baa7c-160">Key of the entity.</span></span> <span data-ttu-id="baa7c-161">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-162">version</span><span class="sxs-lookup"><span data-stu-id="baa7c-162">version</span></span>|<span data-ttu-id="baa7c-163">String</span><span class="sxs-lookup"><span data-stu-id="baa7c-163">String</span></span>|<span data-ttu-id="baa7c-164">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="baa7c-164">Version of the entity.</span></span> <span data-ttu-id="baa7c-165">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="baa7c-166">customSettings</span><span class="sxs-lookup"><span data-stu-id="baa7c-166">customSettings</span></span>|<span data-ttu-id="baa7c-167">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="baa7c-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="baa7c-168">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baa7c-168">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="baa7c-169">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="baa7c-169">deployedAppCount</span></span>|<span data-ttu-id="baa7c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="baa7c-170">Int32</span></span>|<span data-ttu-id="baa7c-171">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="baa7c-171">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="baa7c-172">isAssigned</span><span class="sxs-lookup"><span data-stu-id="baa7c-172">isAssigned</span></span>|<span data-ttu-id="baa7c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa7c-173">Boolean</span></span>|<span data-ttu-id="baa7c-174">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="baa7c-174">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="baa7c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="baa7c-175">Response</span></span>
<span data-ttu-id="baa7c-176">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="baa7c-176">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baa7c-177">Пример</span><span class="sxs-lookup"><span data-stu-id="baa7c-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="baa7c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="baa7c-178">Request</span></span>
<span data-ttu-id="baa7c-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baa7c-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="baa7c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="baa7c-180">Response</span></span>
<span data-ttu-id="baa7c-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baa7c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```







