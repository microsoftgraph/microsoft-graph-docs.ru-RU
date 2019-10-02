---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa070ba00a285890bc0618717f55adb92685db08
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363194"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="0f328-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f328-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="0f328-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f328-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f328-105">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f328-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0f328-106">Prerequisites</span></span>
<span data-ttu-id="0f328-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f328-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f328-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f328-109">Permission type</span></span>|<span data-ttu-id="0f328-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f328-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f328-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f328-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f328-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f328-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f328-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f328-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f328-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f328-114">Not supported.</span></span>|
|<span data-ttu-id="0f328-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f328-115">Application</span></span>|<span data-ttu-id="0f328-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f328-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f328-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f328-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0f328-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f328-118">Request headers</span></span>
|<span data-ttu-id="0f328-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f328-119">Header</span></span>|<span data-ttu-id="0f328-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0f328-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f328-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f328-121">Authorization</span></span>|<span data-ttu-id="0f328-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f328-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f328-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0f328-123">Accept</span></span>|<span data-ttu-id="0f328-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f328-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f328-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f328-125">Request body</span></span>
<span data-ttu-id="0f328-126">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f328-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="0f328-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="0f328-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f328-128">Property</span></span>|<span data-ttu-id="0f328-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0f328-129">Type</span></span>|<span data-ttu-id="0f328-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0f328-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f328-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0f328-131">displayName</span></span>|<span data-ttu-id="0f328-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0f328-132">String</span></span>|<span data-ttu-id="0f328-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0f328-133">Policy display name.</span></span> <span data-ttu-id="0f328-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0f328-135">description</span><span class="sxs-lookup"><span data-stu-id="0f328-135">description</span></span>|<span data-ttu-id="0f328-136">String</span><span class="sxs-lookup"><span data-stu-id="0f328-136">String</span></span>|<span data-ttu-id="0f328-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="0f328-137">The policy's description.</span></span> <span data-ttu-id="0f328-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0f328-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f328-139">createdDateTime</span></span>|<span data-ttu-id="0f328-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f328-140">DateTimeOffset</span></span>|<span data-ttu-id="0f328-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="0f328-141">The date and time the policy was created.</span></span> <span data-ttu-id="0f328-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0f328-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f328-143">lastModifiedDateTime</span></span>|<span data-ttu-id="0f328-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f328-144">DateTimeOffset</span></span>|<span data-ttu-id="0f328-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="0f328-145">Last time the policy was modified.</span></span> <span data-ttu-id="0f328-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0f328-147">id</span><span class="sxs-lookup"><span data-stu-id="0f328-147">id</span></span>|<span data-ttu-id="0f328-148">String</span><span class="sxs-lookup"><span data-stu-id="0f328-148">String</span></span>|<span data-ttu-id="0f328-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f328-149">Key of the entity.</span></span> <span data-ttu-id="0f328-150">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0f328-151">version</span><span class="sxs-lookup"><span data-stu-id="0f328-151">version</span></span>|<span data-ttu-id="0f328-152">String</span><span class="sxs-lookup"><span data-stu-id="0f328-152">String</span></span>|<span data-ttu-id="0f328-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0f328-153">Version of the entity.</span></span> <span data-ttu-id="0f328-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0f328-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="0f328-155">customSettings</span></span>|<span data-ttu-id="0f328-156">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0f328-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0f328-157">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f328-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="0f328-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="0f328-158">deployedAppCount</span></span>|<span data-ttu-id="0f328-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0f328-159">Int32</span></span>|<span data-ttu-id="0f328-160">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="0f328-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="0f328-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f328-161">isAssigned</span></span>|<span data-ttu-id="0f328-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f328-162">Boolean</span></span>|<span data-ttu-id="0f328-163">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="0f328-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="0f328-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f328-164">Response</span></span>
<span data-ttu-id="0f328-165">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f328-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f328-166">Пример</span><span class="sxs-lookup"><span data-stu-id="0f328-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f328-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f328-167">Request</span></span>
<span data-ttu-id="0f328-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f328-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f328-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f328-169">Response</span></span>
<span data-ttu-id="0f328-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f328-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




