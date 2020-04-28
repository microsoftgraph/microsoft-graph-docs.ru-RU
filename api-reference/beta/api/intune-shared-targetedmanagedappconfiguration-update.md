---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8664f6cada95735a51753011c30e19d544341388
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445141"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="5b53b-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b53b-103">Update targetedManagedAppConfiguration</span></span>

<span data-ttu-id="5b53b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b53b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b53b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b53b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b53b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b53b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b53b-107">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b53b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b53b-108">Prerequisites</span></span>
<span data-ttu-id="5b53b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b53b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b53b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b53b-111">Permission type</span></span>|<span data-ttu-id="5b53b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b53b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b53b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b53b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5b53b-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="5b53b-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="5b53b-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b53b-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="5b53b-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5b53b-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="5b53b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b53b-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b53b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b53b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b53b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b53b-119">Not supported.</span></span>|
|<span data-ttu-id="5b53b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b53b-120">Application</span></span>||
| <span data-ttu-id="5b53b-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="5b53b-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="5b53b-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b53b-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="5b53b-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5b53b-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="5b53b-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b53b-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b53b-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b53b-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b53b-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b53b-126">Request headers</span></span>
|<span data-ttu-id="5b53b-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b53b-127">Header</span></span>|<span data-ttu-id="5b53b-128">Значение</span><span class="sxs-lookup"><span data-stu-id="5b53b-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b53b-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b53b-129">Authorization</span></span>|<span data-ttu-id="5b53b-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b53b-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b53b-131">Accept</span><span class="sxs-lookup"><span data-stu-id="5b53b-131">Accept</span></span>|<span data-ttu-id="5b53b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5b53b-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b53b-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b53b-133">Request body</span></span>
<span data-ttu-id="5b53b-134">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b53b-134">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="5b53b-135">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-135">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="5b53b-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b53b-136">Property</span></span>|<span data-ttu-id="5b53b-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5b53b-137">Type</span></span>|<span data-ttu-id="5b53b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5b53b-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b53b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5b53b-139">displayName</span></span>|<span data-ttu-id="5b53b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5b53b-140">String</span></span>|<span data-ttu-id="5b53b-141">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="5b53b-141">Policy display name.</span></span> <span data-ttu-id="5b53b-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-143">description</span><span class="sxs-lookup"><span data-stu-id="5b53b-143">description</span></span>|<span data-ttu-id="5b53b-144">String</span><span class="sxs-lookup"><span data-stu-id="5b53b-144">String</span></span>|<span data-ttu-id="5b53b-145">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="5b53b-145">The policy's description.</span></span> <span data-ttu-id="5b53b-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b53b-147">createdDateTime</span></span>|<span data-ttu-id="5b53b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b53b-148">DateTimeOffset</span></span>|<span data-ttu-id="5b53b-149">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="5b53b-149">The date and time the policy was created.</span></span> <span data-ttu-id="5b53b-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b53b-151">lastModifiedDateTime</span></span>|<span data-ttu-id="5b53b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b53b-152">DateTimeOffset</span></span>|<span data-ttu-id="5b53b-153">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="5b53b-153">Last time the policy was modified.</span></span> <span data-ttu-id="5b53b-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b53b-155">roleScopeTagIds</span></span>|<span data-ttu-id="5b53b-156">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5b53b-156">String collection</span></span>|<span data-ttu-id="5b53b-157">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5b53b-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b53b-158">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-159">id</span><span class="sxs-lookup"><span data-stu-id="5b53b-159">id</span></span>|<span data-ttu-id="5b53b-160">String</span><span class="sxs-lookup"><span data-stu-id="5b53b-160">String</span></span>|<span data-ttu-id="5b53b-161">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b53b-161">Key of the entity.</span></span> <span data-ttu-id="5b53b-162">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-163">version</span><span class="sxs-lookup"><span data-stu-id="5b53b-163">version</span></span>|<span data-ttu-id="5b53b-164">String</span><span class="sxs-lookup"><span data-stu-id="5b53b-164">String</span></span>|<span data-ttu-id="5b53b-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5b53b-165">Version of the entity.</span></span> <span data-ttu-id="5b53b-166">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5b53b-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="5b53b-167">customSettings</span></span>|<span data-ttu-id="5b53b-168">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5b53b-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5b53b-169">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b53b-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="5b53b-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="5b53b-170">deployedAppCount</span></span>|<span data-ttu-id="5b53b-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5b53b-171">Int32</span></span>|<span data-ttu-id="5b53b-172">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="5b53b-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="5b53b-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5b53b-173">isAssigned</span></span>|<span data-ttu-id="5b53b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b53b-174">Boolean</span></span>|<span data-ttu-id="5b53b-175">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="5b53b-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="5b53b-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b53b-176">Response</span></span>
<span data-ttu-id="5b53b-177">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b53b-177">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b53b-178">Пример</span><span class="sxs-lookup"><span data-stu-id="5b53b-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b53b-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b53b-179">Request</span></span>
<span data-ttu-id="5b53b-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b53b-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b53b-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b53b-181">Response</span></span>
<span data-ttu-id="5b53b-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b53b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






