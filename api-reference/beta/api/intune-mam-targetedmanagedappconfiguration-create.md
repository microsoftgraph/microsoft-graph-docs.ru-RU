---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f98fa738833d70c871806f7557dc9289720a211
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994490"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="5c6b4-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c6b4-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="5c6b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c6b4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c6b4-106">Создание объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c6b4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c6b4-107">Prerequisites</span></span>
<span data-ttu-id="5c6b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c6b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c6b4-110">Permission type</span></span>|<span data-ttu-id="5c6b4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c6b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c6b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c6b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c6b4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6b4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c6b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c6b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c6b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-115">Not supported.</span></span>|
|<span data-ttu-id="5c6b4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c6b4-116">Application</span></span>|<span data-ttu-id="5c6b4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c6b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c6b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c6b4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c6b4-119">Request headers</span></span>
|<span data-ttu-id="5c6b4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c6b4-120">Header</span></span>|<span data-ttu-id="5c6b4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c6b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c6b4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c6b4-122">Authorization</span></span>|<span data-ttu-id="5c6b4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c6b4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c6b4-124">Accept</span></span>|<span data-ttu-id="5c6b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c6b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c6b4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c6b4-126">Request body</span></span>
<span data-ttu-id="5c6b4-127">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="5c6b4-128">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="5c6b4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c6b4-129">Property</span></span>|<span data-ttu-id="5c6b4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c6b4-130">Type</span></span>|<span data-ttu-id="5c6b4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c6b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c6b4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5c6b4-132">displayName</span></span>|<span data-ttu-id="5c6b4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5c6b4-133">String</span></span>|<span data-ttu-id="5c6b4-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-134">Policy display name.</span></span> <span data-ttu-id="5c6b4-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-136">description</span><span class="sxs-lookup"><span data-stu-id="5c6b4-136">description</span></span>|<span data-ttu-id="5c6b4-137">String</span><span class="sxs-lookup"><span data-stu-id="5c6b4-137">String</span></span>|<span data-ttu-id="5c6b4-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-138">The policy's description.</span></span> <span data-ttu-id="5c6b4-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c6b4-140">createdDateTime</span></span>|<span data-ttu-id="5c6b4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c6b4-141">DateTimeOffset</span></span>|<span data-ttu-id="5c6b4-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-142">The date and time the policy was created.</span></span> <span data-ttu-id="5c6b4-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c6b4-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5c6b4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c6b4-145">DateTimeOffset</span></span>|<span data-ttu-id="5c6b4-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-146">Last time the policy was modified.</span></span> <span data-ttu-id="5c6b4-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c6b4-148">roleScopeTagIds</span></span>|<span data-ttu-id="5c6b4-149">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5c6b4-149">String collection</span></span>|<span data-ttu-id="5c6b4-150">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c6b4-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-152">id</span><span class="sxs-lookup"><span data-stu-id="5c6b4-152">id</span></span>|<span data-ttu-id="5c6b4-153">String</span><span class="sxs-lookup"><span data-stu-id="5c6b4-153">String</span></span>|<span data-ttu-id="5c6b4-154">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-154">Key of the entity.</span></span> <span data-ttu-id="5c6b4-155">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-156">version</span><span class="sxs-lookup"><span data-stu-id="5c6b4-156">version</span></span>|<span data-ttu-id="5c6b4-157">String</span><span class="sxs-lookup"><span data-stu-id="5c6b4-157">String</span></span>|<span data-ttu-id="5c6b4-158">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-158">Version of the entity.</span></span> <span data-ttu-id="5c6b4-159">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c6b4-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="5c6b4-160">customSettings</span></span>|<span data-ttu-id="5c6b4-161">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5c6b4-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5c6b4-162">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c6b4-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="5c6b4-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="5c6b4-163">deployedAppCount</span></span>|<span data-ttu-id="5c6b4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5c6b4-164">Int32</span></span>|<span data-ttu-id="5c6b4-165">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="5c6b4-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5c6b4-166">isAssigned</span></span>|<span data-ttu-id="5c6b4-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c6b4-167">Boolean</span></span>|<span data-ttu-id="5c6b4-168">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="5c6b4-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c6b4-169">Response</span></span>
<span data-ttu-id="5c6b4-170">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-170">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c6b4-171">Пример</span><span class="sxs-lookup"><span data-stu-id="5c6b4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c6b4-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c6b4-172">Request</span></span>
<span data-ttu-id="5c6b4-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c6b4-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c6b4-174">Response</span></span>
<span data-ttu-id="5c6b4-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c6b4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





