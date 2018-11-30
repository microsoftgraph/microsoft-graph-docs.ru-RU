---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
ms.openlocfilehash: 2157c6bb07562ca3aaff1a15737ec5dc6a7f19bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028113"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="e3e25-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e3e25-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="e3e25-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3e25-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3e25-105">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3e25-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e3e25-106">Prerequisites</span></span>
<span data-ttu-id="e3e25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3e25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3e25-109">Permission type</span></span>|<span data-ttu-id="e3e25-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3e25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3e25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e25-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e25-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3e25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3e25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e25-114">Not supported.</span></span>|
|<span data-ttu-id="e3e25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3e25-115">Application</span></span>|<span data-ttu-id="e3e25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3e25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3e25-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e3e25-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3e25-118">Request headers</span></span>
|<span data-ttu-id="e3e25-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3e25-119">Header</span></span>|<span data-ttu-id="e3e25-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e3e25-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e25-121">Authorization</span></span>|<span data-ttu-id="e3e25-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3e25-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e25-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3e25-123">Accept</span></span>|<span data-ttu-id="e3e25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e25-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e25-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3e25-125">Request body</span></span>
<span data-ttu-id="e3e25-126">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3e25-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="e3e25-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="e3e25-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3e25-128">Property</span></span>|<span data-ttu-id="e3e25-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e3e25-129">Type</span></span>|<span data-ttu-id="e3e25-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e3e25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e25-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e3e25-131">displayName</span></span>|<span data-ttu-id="e3e25-132">String</span><span class="sxs-lookup"><span data-stu-id="e3e25-132">String</span></span>|<span data-ttu-id="e3e25-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="e3e25-133">Policy display name.</span></span> <span data-ttu-id="e3e25-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e3e25-135">описание</span><span class="sxs-lookup"><span data-stu-id="e3e25-135">description</span></span>|<span data-ttu-id="e3e25-136">String</span><span class="sxs-lookup"><span data-stu-id="e3e25-136">String</span></span>|<span data-ttu-id="e3e25-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="e3e25-137">The policy's description.</span></span> <span data-ttu-id="e3e25-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e3e25-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e25-139">createdDateTime</span></span>|<span data-ttu-id="e3e25-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e25-140">DateTimeOffset</span></span>|<span data-ttu-id="e3e25-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="e3e25-141">The date and time the policy was created.</span></span> <span data-ttu-id="e3e25-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e3e25-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e25-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e3e25-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e25-144">DateTimeOffset</span></span>|<span data-ttu-id="e3e25-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="e3e25-145">Last time the policy was modified.</span></span> <span data-ttu-id="e3e25-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e3e25-147">id</span><span class="sxs-lookup"><span data-stu-id="e3e25-147">id</span></span>|<span data-ttu-id="e3e25-148">String</span><span class="sxs-lookup"><span data-stu-id="e3e25-148">String</span></span>|<span data-ttu-id="e3e25-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3e25-149">Key of the entity.</span></span> <span data-ttu-id="e3e25-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e3e25-151">version</span><span class="sxs-lookup"><span data-stu-id="e3e25-151">version</span></span>|<span data-ttu-id="e3e25-152">String</span><span class="sxs-lookup"><span data-stu-id="e3e25-152">String</span></span>|<span data-ttu-id="e3e25-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e3e25-153">Version of the entity.</span></span> <span data-ttu-id="e3e25-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e3e25-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="e3e25-155">customSettings</span></span>|<span data-ttu-id="e3e25-156">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e3e25-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e3e25-157">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3e25-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="e3e25-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="e3e25-158">deployedAppCount</span></span>|<span data-ttu-id="e3e25-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e25-159">Int32</span></span>|<span data-ttu-id="e3e25-160">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="e3e25-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="e3e25-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e3e25-161">isAssigned</span></span>|<span data-ttu-id="e3e25-162">Логический</span><span class="sxs-lookup"><span data-stu-id="e3e25-162">Boolean</span></span>|<span data-ttu-id="e3e25-163">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="e3e25-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="e3e25-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3e25-164">Response</span></span>
<span data-ttu-id="e3e25-165">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3e25-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e25-166">Пример</span><span class="sxs-lookup"><span data-stu-id="e3e25-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3e25-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3e25-167">Request</span></span>
<span data-ttu-id="e3e25-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3e25-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="e3e25-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3e25-169">Response</span></span>
<span data-ttu-id="e3e25-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e3e25-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



