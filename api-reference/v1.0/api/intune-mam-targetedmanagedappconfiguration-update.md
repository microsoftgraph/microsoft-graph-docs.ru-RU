---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1a07d46298c31f5fff1cd820888828175936838
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978995"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="052df-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="052df-103">Update targetedManagedAppConfiguration</span></span>

<span data-ttu-id="052df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="052df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="052df-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="052df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="052df-106">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="052df-106">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="052df-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="052df-107">Prerequisites</span></span>
<span data-ttu-id="052df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="052df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="052df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="052df-110">Permission type</span></span>|<span data-ttu-id="052df-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="052df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="052df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="052df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="052df-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="052df-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="052df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="052df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="052df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="052df-115">Not supported.</span></span>|
|<span data-ttu-id="052df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="052df-116">Application</span></span>|<span data-ttu-id="052df-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="052df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="052df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="052df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="052df-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="052df-119">Request headers</span></span>
|<span data-ttu-id="052df-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="052df-120">Header</span></span>|<span data-ttu-id="052df-121">Значение</span><span class="sxs-lookup"><span data-stu-id="052df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="052df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="052df-122">Authorization</span></span>|<span data-ttu-id="052df-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="052df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="052df-124">Accept</span><span class="sxs-lookup"><span data-stu-id="052df-124">Accept</span></span>|<span data-ttu-id="052df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="052df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="052df-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="052df-126">Request body</span></span>
<span data-ttu-id="052df-127">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="052df-127">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="052df-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="052df-128">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="052df-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="052df-129">Property</span></span>|<span data-ttu-id="052df-130">Тип</span><span class="sxs-lookup"><span data-stu-id="052df-130">Type</span></span>|<span data-ttu-id="052df-131">Описание</span><span class="sxs-lookup"><span data-stu-id="052df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="052df-132">displayName</span><span class="sxs-lookup"><span data-stu-id="052df-132">displayName</span></span>|<span data-ttu-id="052df-133">String</span><span class="sxs-lookup"><span data-stu-id="052df-133">String</span></span>|<span data-ttu-id="052df-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="052df-134">Policy display name.</span></span> <span data-ttu-id="052df-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="052df-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="052df-136">description</span><span class="sxs-lookup"><span data-stu-id="052df-136">description</span></span>|<span data-ttu-id="052df-137">String</span><span class="sxs-lookup"><span data-stu-id="052df-137">String</span></span>|<span data-ttu-id="052df-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="052df-138">The policy's description.</span></span> <span data-ttu-id="052df-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="052df-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="052df-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="052df-140">createdDateTime</span></span>|<span data-ttu-id="052df-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="052df-141">DateTimeOffset</span></span>|<span data-ttu-id="052df-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="052df-142">The date and time the policy was created.</span></span> <span data-ttu-id="052df-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="052df-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="052df-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="052df-144">lastModifiedDateTime</span></span>|<span data-ttu-id="052df-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="052df-145">DateTimeOffset</span></span>|<span data-ttu-id="052df-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="052df-146">Last time the policy was modified.</span></span> <span data-ttu-id="052df-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="052df-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="052df-148">id</span><span class="sxs-lookup"><span data-stu-id="052df-148">id</span></span>|<span data-ttu-id="052df-149">String</span><span class="sxs-lookup"><span data-stu-id="052df-149">String</span></span>|<span data-ttu-id="052df-150">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="052df-150">Key of the entity.</span></span> <span data-ttu-id="052df-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="052df-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="052df-152">version</span><span class="sxs-lookup"><span data-stu-id="052df-152">version</span></span>|<span data-ttu-id="052df-153">String</span><span class="sxs-lookup"><span data-stu-id="052df-153">String</span></span>|<span data-ttu-id="052df-154">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="052df-154">Version of the entity.</span></span> <span data-ttu-id="052df-155">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="052df-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="052df-156">customSettings</span><span class="sxs-lookup"><span data-stu-id="052df-156">customSettings</span></span>|<span data-ttu-id="052df-157">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="052df-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="052df-158">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="052df-158">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="052df-159">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="052df-159">deployedAppCount</span></span>|<span data-ttu-id="052df-160">Int32</span><span class="sxs-lookup"><span data-stu-id="052df-160">Int32</span></span>|<span data-ttu-id="052df-161">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="052df-161">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="052df-162">isAssigned</span><span class="sxs-lookup"><span data-stu-id="052df-162">isAssigned</span></span>|<span data-ttu-id="052df-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="052df-163">Boolean</span></span>|<span data-ttu-id="052df-164">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="052df-164">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="052df-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="052df-165">Response</span></span>
<span data-ttu-id="052df-166">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="052df-166">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="052df-167">Пример</span><span class="sxs-lookup"><span data-stu-id="052df-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="052df-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="052df-168">Request</span></span>
<span data-ttu-id="052df-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="052df-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="052df-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="052df-170">Response</span></span>
<span data-ttu-id="052df-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="052df-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









