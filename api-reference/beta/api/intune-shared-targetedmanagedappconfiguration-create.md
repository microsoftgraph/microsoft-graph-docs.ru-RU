---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fd5f17872d848f91e7a1dcaeb7b150c44901c93
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201156"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="285a9-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="285a9-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="285a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="285a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="285a9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="285a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="285a9-106">Создание объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-106">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="285a9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="285a9-107">Prerequisites</span></span>
<span data-ttu-id="285a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="285a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="285a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="285a9-110">Permission type</span></span>|<span data-ttu-id="285a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="285a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="285a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="285a9-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="285a9-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="285a9-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="285a9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285a9-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="285a9-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="285a9-115">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="285a9-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285a9-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="285a9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="285a9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="285a9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="285a9-118">Not supported.</span></span>|
|<span data-ttu-id="285a9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="285a9-119">Application</span></span>||
| <span data-ttu-id="285a9-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="285a9-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="285a9-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285a9-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="285a9-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="285a9-122">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="285a9-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285a9-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="285a9-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="285a9-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="285a9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="285a9-125">Request headers</span></span>
|<span data-ttu-id="285a9-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="285a9-126">Header</span></span>|<span data-ttu-id="285a9-127">Значение</span><span class="sxs-lookup"><span data-stu-id="285a9-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="285a9-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="285a9-128">Authorization</span></span>|<span data-ttu-id="285a9-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="285a9-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="285a9-130">Accept</span><span class="sxs-lookup"><span data-stu-id="285a9-130">Accept</span></span>|<span data-ttu-id="285a9-131">application/json</span><span class="sxs-lookup"><span data-stu-id="285a9-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="285a9-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="285a9-132">Request body</span></span>
<span data-ttu-id="285a9-133">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="285a9-133">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="285a9-134">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="285a9-134">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="285a9-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="285a9-135">Property</span></span>|<span data-ttu-id="285a9-136">Тип</span><span class="sxs-lookup"><span data-stu-id="285a9-136">Type</span></span>|<span data-ttu-id="285a9-137">Описание</span><span class="sxs-lookup"><span data-stu-id="285a9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="285a9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="285a9-138">displayName</span></span>|<span data-ttu-id="285a9-139">Строка</span><span class="sxs-lookup"><span data-stu-id="285a9-139">String</span></span>|<span data-ttu-id="285a9-140">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="285a9-140">Policy display name.</span></span> <span data-ttu-id="285a9-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-142">description</span><span class="sxs-lookup"><span data-stu-id="285a9-142">description</span></span>|<span data-ttu-id="285a9-143">String</span><span class="sxs-lookup"><span data-stu-id="285a9-143">String</span></span>|<span data-ttu-id="285a9-144">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="285a9-144">The policy's description.</span></span> <span data-ttu-id="285a9-145">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="285a9-146">createdDateTime</span></span>|<span data-ttu-id="285a9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="285a9-147">DateTimeOffset</span></span>|<span data-ttu-id="285a9-148">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="285a9-148">The date and time the policy was created.</span></span> <span data-ttu-id="285a9-149">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="285a9-150">lastModifiedDateTime</span></span>|<span data-ttu-id="285a9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="285a9-151">DateTimeOffset</span></span>|<span data-ttu-id="285a9-152">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="285a9-152">Last time the policy was modified.</span></span> <span data-ttu-id="285a9-153">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="285a9-154">roleScopeTagIds</span></span>|<span data-ttu-id="285a9-155">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="285a9-155">String collection</span></span>|<span data-ttu-id="285a9-156">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="285a9-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="285a9-157">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-158">id</span><span class="sxs-lookup"><span data-stu-id="285a9-158">id</span></span>|<span data-ttu-id="285a9-159">String.</span><span class="sxs-lookup"><span data-stu-id="285a9-159">String</span></span>|<span data-ttu-id="285a9-160">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="285a9-160">Key of the entity.</span></span> <span data-ttu-id="285a9-161">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-162">version</span><span class="sxs-lookup"><span data-stu-id="285a9-162">version</span></span>|<span data-ttu-id="285a9-163">String</span><span class="sxs-lookup"><span data-stu-id="285a9-163">String</span></span>|<span data-ttu-id="285a9-164">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="285a9-164">Version of the entity.</span></span> <span data-ttu-id="285a9-165">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="285a9-166">customSettings</span><span class="sxs-lookup"><span data-stu-id="285a9-166">customSettings</span></span>|<span data-ttu-id="285a9-167">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="285a9-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="285a9-168">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="285a9-168">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="285a9-169">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="285a9-169">deployedAppCount</span></span>|<span data-ttu-id="285a9-170">Int32</span><span class="sxs-lookup"><span data-stu-id="285a9-170">Int32</span></span>|<span data-ttu-id="285a9-171">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="285a9-171">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="285a9-172">isAssigned</span><span class="sxs-lookup"><span data-stu-id="285a9-172">isAssigned</span></span>|<span data-ttu-id="285a9-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="285a9-173">Boolean</span></span>|<span data-ttu-id="285a9-174">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="285a9-174">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="285a9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="285a9-175">Response</span></span>
<span data-ttu-id="285a9-176">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="285a9-176">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="285a9-177">Пример</span><span class="sxs-lookup"><span data-stu-id="285a9-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="285a9-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="285a9-178">Request</span></span>
<span data-ttu-id="285a9-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="285a9-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="285a9-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="285a9-180">Response</span></span>
<span data-ttu-id="285a9-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="285a9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




