---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eded21015054073b6f6711faecd5c01da52fece0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403695"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="9ff37-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ff37-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="9ff37-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ff37-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ff37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ff37-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ff37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff37-107">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ff37-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9ff37-108">Prerequisites</span></span>
<span data-ttu-id="9ff37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ff37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ff37-111">Permission type</span></span>|<span data-ttu-id="9ff37-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ff37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ff37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ff37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ff37-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff37-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ff37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ff37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ff37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff37-116">Not supported.</span></span>|
|<span data-ttu-id="9ff37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ff37-117">Application</span></span>|<span data-ttu-id="9ff37-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ff37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ff37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ff37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ff37-120">Request headers</span></span>
|<span data-ttu-id="9ff37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ff37-121">Header</span></span>|<span data-ttu-id="9ff37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ff37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ff37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ff37-123">Authorization</span></span>|<span data-ttu-id="9ff37-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9ff37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ff37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ff37-125">Accept</span></span>|<span data-ttu-id="9ff37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ff37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff37-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ff37-127">Request body</span></span>
<span data-ttu-id="9ff37-128">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ff37-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="9ff37-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="9ff37-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ff37-130">Property</span></span>|<span data-ttu-id="9ff37-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9ff37-131">Type</span></span>|<span data-ttu-id="9ff37-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff37-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9ff37-133">displayName</span></span>|<span data-ttu-id="9ff37-134">String</span><span class="sxs-lookup"><span data-stu-id="9ff37-134">String</span></span>|<span data-ttu-id="9ff37-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="9ff37-135">Policy display name.</span></span> <span data-ttu-id="9ff37-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-137">description</span><span class="sxs-lookup"><span data-stu-id="9ff37-137">description</span></span>|<span data-ttu-id="9ff37-138">String</span><span class="sxs-lookup"><span data-stu-id="9ff37-138">String</span></span>|<span data-ttu-id="9ff37-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="9ff37-139">The policy's description.</span></span> <span data-ttu-id="9ff37-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff37-141">createdDateTime</span></span>|<span data-ttu-id="9ff37-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff37-142">DateTimeOffset</span></span>|<span data-ttu-id="9ff37-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="9ff37-143">The date and time the policy was created.</span></span> <span data-ttu-id="9ff37-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff37-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9ff37-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff37-146">DateTimeOffset</span></span>|<span data-ttu-id="9ff37-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="9ff37-147">Last time the policy was modified.</span></span> <span data-ttu-id="9ff37-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ff37-149">roleScopeTagIds</span></span>|<span data-ttu-id="9ff37-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9ff37-150">String collection</span></span>|<span data-ttu-id="9ff37-151">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9ff37-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ff37-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-153">id</span><span class="sxs-lookup"><span data-stu-id="9ff37-153">id</span></span>|<span data-ttu-id="9ff37-154">String</span><span class="sxs-lookup"><span data-stu-id="9ff37-154">String</span></span>|<span data-ttu-id="9ff37-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ff37-155">Key of the entity.</span></span> <span data-ttu-id="9ff37-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-157">version</span><span class="sxs-lookup"><span data-stu-id="9ff37-157">version</span></span>|<span data-ttu-id="9ff37-158">String</span><span class="sxs-lookup"><span data-stu-id="9ff37-158">String</span></span>|<span data-ttu-id="9ff37-159">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9ff37-159">Version of the entity.</span></span> <span data-ttu-id="9ff37-160">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9ff37-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="9ff37-161">customSettings</span></span>|<span data-ttu-id="9ff37-162">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9ff37-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9ff37-163">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff37-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="9ff37-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="9ff37-164">deployedAppCount</span></span>|<span data-ttu-id="9ff37-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff37-165">Int32</span></span>|<span data-ttu-id="9ff37-166">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="9ff37-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="9ff37-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ff37-167">isAssigned</span></span>|<span data-ttu-id="9ff37-168">Логический</span><span class="sxs-lookup"><span data-stu-id="9ff37-168">Boolean</span></span>|<span data-ttu-id="9ff37-169">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="9ff37-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="9ff37-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ff37-170">Response</span></span>
<span data-ttu-id="9ff37-171">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9ff37-171">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff37-172">Пример</span><span class="sxs-lookup"><span data-stu-id="9ff37-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ff37-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ff37-173">Request</span></span>
<span data-ttu-id="9ff37-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ff37-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ff37-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ff37-175">Response</span></span>
<span data-ttu-id="9ff37-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9ff37-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




