---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2cc769d7bf30c41ac717cabc74c373136a06847
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723109"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="dd679-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd679-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="dd679-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd679-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd679-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd679-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd679-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd679-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd679-107">Создание объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-107">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd679-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd679-108">Prerequisites</span></span>
<span data-ttu-id="dd679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd679-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd679-111">Permission type</span></span>|<span data-ttu-id="dd679-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd679-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd679-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd679-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dd679-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="dd679-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="dd679-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd679-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="dd679-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="dd679-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="dd679-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd679-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd679-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd679-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd679-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd679-119">Not supported.</span></span>|
|<span data-ttu-id="dd679-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd679-120">Application</span></span>||
| <span data-ttu-id="dd679-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="dd679-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="dd679-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd679-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="dd679-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="dd679-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="dd679-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd679-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd679-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd679-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dd679-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd679-126">Request headers</span></span>
|<span data-ttu-id="dd679-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd679-127">Header</span></span>|<span data-ttu-id="dd679-128">Значение</span><span class="sxs-lookup"><span data-stu-id="dd679-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd679-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd679-129">Authorization</span></span>|<span data-ttu-id="dd679-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd679-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd679-131">Accept</span><span class="sxs-lookup"><span data-stu-id="dd679-131">Accept</span></span>|<span data-ttu-id="dd679-132">application/json</span><span class="sxs-lookup"><span data-stu-id="dd679-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd679-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd679-133">Request body</span></span>
<span data-ttu-id="dd679-134">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd679-134">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="dd679-135">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dd679-135">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="dd679-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd679-136">Property</span></span>|<span data-ttu-id="dd679-137">Тип</span><span class="sxs-lookup"><span data-stu-id="dd679-137">Type</span></span>|<span data-ttu-id="dd679-138">Описание</span><span class="sxs-lookup"><span data-stu-id="dd679-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd679-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dd679-139">displayName</span></span>|<span data-ttu-id="dd679-140">Строка</span><span class="sxs-lookup"><span data-stu-id="dd679-140">String</span></span>|<span data-ttu-id="dd679-141">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="dd679-141">Policy display name.</span></span> <span data-ttu-id="dd679-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-143">description</span><span class="sxs-lookup"><span data-stu-id="dd679-143">description</span></span>|<span data-ttu-id="dd679-144">Строка</span><span class="sxs-lookup"><span data-stu-id="dd679-144">String</span></span>|<span data-ttu-id="dd679-145">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="dd679-145">The policy's description.</span></span> <span data-ttu-id="dd679-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd679-147">createdDateTime</span></span>|<span data-ttu-id="dd679-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd679-148">DateTimeOffset</span></span>|<span data-ttu-id="dd679-149">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="dd679-149">The date and time the policy was created.</span></span> <span data-ttu-id="dd679-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd679-151">lastModifiedDateTime</span></span>|<span data-ttu-id="dd679-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd679-152">DateTimeOffset</span></span>|<span data-ttu-id="dd679-153">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="dd679-153">Last time the policy was modified.</span></span> <span data-ttu-id="dd679-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd679-155">roleScopeTagIds</span></span>|<span data-ttu-id="dd679-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dd679-156">String collection</span></span>|<span data-ttu-id="dd679-157">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dd679-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd679-158">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-159">id</span><span class="sxs-lookup"><span data-stu-id="dd679-159">id</span></span>|<span data-ttu-id="dd679-160">Строка</span><span class="sxs-lookup"><span data-stu-id="dd679-160">String</span></span>|<span data-ttu-id="dd679-161">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd679-161">Key of the entity.</span></span> <span data-ttu-id="dd679-162">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-163">version</span><span class="sxs-lookup"><span data-stu-id="dd679-163">version</span></span>|<span data-ttu-id="dd679-164">String</span><span class="sxs-lookup"><span data-stu-id="dd679-164">String</span></span>|<span data-ttu-id="dd679-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="dd679-165">Version of the entity.</span></span> <span data-ttu-id="dd679-166">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="dd679-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="dd679-167">customSettings</span></span>|<span data-ttu-id="dd679-168">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="dd679-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="dd679-169">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd679-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="dd679-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="dd679-170">deployedAppCount</span></span>|<span data-ttu-id="dd679-171">Int32</span><span class="sxs-lookup"><span data-stu-id="dd679-171">Int32</span></span>|<span data-ttu-id="dd679-172">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="dd679-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="dd679-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dd679-173">isAssigned</span></span>|<span data-ttu-id="dd679-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd679-174">Boolean</span></span>|<span data-ttu-id="dd679-175">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="dd679-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="dd679-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd679-176">Response</span></span>
<span data-ttu-id="dd679-177">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd679-177">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd679-178">Пример</span><span class="sxs-lookup"><span data-stu-id="dd679-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd679-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd679-179">Request</span></span>
<span data-ttu-id="dd679-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd679-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
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

### <a name="response"></a><span data-ttu-id="dd679-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd679-181">Response</span></span>
<span data-ttu-id="dd679-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd679-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








