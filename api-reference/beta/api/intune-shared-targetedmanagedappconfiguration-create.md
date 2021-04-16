---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e4d3116c4fabc7880f680eb73754c54a4747bdc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866680"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="2b726-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b726-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="2b726-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b726-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b726-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b726-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b726-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b726-107">Создание объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-107">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b726-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b726-108">Prerequisites</span></span>
<span data-ttu-id="2b726-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b726-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b726-111">Permission type</span></span>|<span data-ttu-id="2b726-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b726-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b726-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b726-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2b726-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="2b726-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2b726-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b726-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2b726-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2b726-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="2b726-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b726-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2b726-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b726-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b726-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b726-119">Not supported.</span></span>|
|<span data-ttu-id="2b726-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2b726-120">Application</span></span>||
| <span data-ttu-id="2b726-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="2b726-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2b726-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b726-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2b726-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2b726-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="2b726-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b726-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b726-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b726-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b726-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b726-126">Request headers</span></span>
|<span data-ttu-id="2b726-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b726-127">Header</span></span>|<span data-ttu-id="2b726-128">Значение</span><span class="sxs-lookup"><span data-stu-id="2b726-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b726-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b726-129">Authorization</span></span>|<span data-ttu-id="2b726-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b726-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b726-131">Accept</span><span class="sxs-lookup"><span data-stu-id="2b726-131">Accept</span></span>|<span data-ttu-id="2b726-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2b726-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b726-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b726-133">Request body</span></span>
<span data-ttu-id="2b726-134">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b726-134">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="2b726-135">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2b726-135">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="2b726-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b726-136">Property</span></span>|<span data-ttu-id="2b726-137">Тип</span><span class="sxs-lookup"><span data-stu-id="2b726-137">Type</span></span>|<span data-ttu-id="2b726-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2b726-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b726-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2b726-139">displayName</span></span>|<span data-ttu-id="2b726-140">String</span><span class="sxs-lookup"><span data-stu-id="2b726-140">String</span></span>|<span data-ttu-id="2b726-141">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="2b726-141">Policy display name.</span></span> <span data-ttu-id="2b726-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-143">description</span><span class="sxs-lookup"><span data-stu-id="2b726-143">description</span></span>|<span data-ttu-id="2b726-144">String</span><span class="sxs-lookup"><span data-stu-id="2b726-144">String</span></span>|<span data-ttu-id="2b726-145">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="2b726-145">The policy's description.</span></span> <span data-ttu-id="2b726-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b726-147">createdDateTime</span></span>|<span data-ttu-id="2b726-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b726-148">DateTimeOffset</span></span>|<span data-ttu-id="2b726-149">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="2b726-149">The date and time the policy was created.</span></span> <span data-ttu-id="2b726-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b726-151">lastModifiedDateTime</span></span>|<span data-ttu-id="2b726-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b726-152">DateTimeOffset</span></span>|<span data-ttu-id="2b726-153">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="2b726-153">Last time the policy was modified.</span></span> <span data-ttu-id="2b726-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b726-155">roleScopeTagIds</span></span>|<span data-ttu-id="2b726-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b726-156">String collection</span></span>|<span data-ttu-id="2b726-157">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="2b726-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b726-158">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-159">id</span><span class="sxs-lookup"><span data-stu-id="2b726-159">id</span></span>|<span data-ttu-id="2b726-160">String</span><span class="sxs-lookup"><span data-stu-id="2b726-160">String</span></span>|<span data-ttu-id="2b726-161">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b726-161">Key of the entity.</span></span> <span data-ttu-id="2b726-162">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-163">version</span><span class="sxs-lookup"><span data-stu-id="2b726-163">version</span></span>|<span data-ttu-id="2b726-164">String</span><span class="sxs-lookup"><span data-stu-id="2b726-164">String</span></span>|<span data-ttu-id="2b726-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="2b726-165">Version of the entity.</span></span> <span data-ttu-id="2b726-166">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2b726-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="2b726-167">customSettings</span></span>|<span data-ttu-id="2b726-168">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2b726-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2b726-169">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b726-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="2b726-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="2b726-170">deployedAppCount</span></span>|<span data-ttu-id="2b726-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2b726-171">Int32</span></span>|<span data-ttu-id="2b726-172">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="2b726-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="2b726-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2b726-173">isAssigned</span></span>|<span data-ttu-id="2b726-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b726-174">Boolean</span></span>|<span data-ttu-id="2b726-175">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="2b726-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="2b726-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b726-176">Response</span></span>
<span data-ttu-id="2b726-177">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b726-177">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b726-178">Пример</span><span class="sxs-lookup"><span data-stu-id="2b726-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b726-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b726-179">Request</span></span>
<span data-ttu-id="2b726-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b726-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b726-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b726-181">Response</span></span>
<span data-ttu-id="2b726-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b726-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







