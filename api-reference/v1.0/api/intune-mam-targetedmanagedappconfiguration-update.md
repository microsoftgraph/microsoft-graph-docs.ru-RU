---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7e811ad24c2a91f3b95ae3e6deb7e949b069035
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583195"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="202b3-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="202b3-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="202b3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="202b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="202b3-105">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="202b3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="202b3-106">Prerequisites</span></span>
<span data-ttu-id="202b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="202b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202b3-109">Permission type</span></span>|<span data-ttu-id="202b3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="202b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="202b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="202b3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="202b3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="202b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="202b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202b3-114">Not supported.</span></span>|
|<span data-ttu-id="202b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202b3-115">Application</span></span>|<span data-ttu-id="202b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="202b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="202b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="202b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="202b3-118">Request headers</span></span>
|<span data-ttu-id="202b3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="202b3-119">Header</span></span>|<span data-ttu-id="202b3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="202b3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="202b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="202b3-121">Authorization</span></span>|<span data-ttu-id="202b3-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="202b3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="202b3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="202b3-123">Accept</span></span>|<span data-ttu-id="202b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="202b3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="202b3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="202b3-125">Request body</span></span>
<span data-ttu-id="202b3-126">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="202b3-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="202b3-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="202b3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="202b3-128">Property</span></span>|<span data-ttu-id="202b3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="202b3-129">Type</span></span>|<span data-ttu-id="202b3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="202b3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="202b3-131">displayName</span><span class="sxs-lookup"><span data-stu-id="202b3-131">displayName</span></span>|<span data-ttu-id="202b3-132">String</span><span class="sxs-lookup"><span data-stu-id="202b3-132">String</span></span>|<span data-ttu-id="202b3-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="202b3-133">Policy display name.</span></span> <span data-ttu-id="202b3-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="202b3-135">description</span><span class="sxs-lookup"><span data-stu-id="202b3-135">description</span></span>|<span data-ttu-id="202b3-136">String</span><span class="sxs-lookup"><span data-stu-id="202b3-136">String</span></span>|<span data-ttu-id="202b3-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="202b3-137">The policy's description.</span></span> <span data-ttu-id="202b3-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="202b3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="202b3-139">createdDateTime</span></span>|<span data-ttu-id="202b3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="202b3-140">DateTimeOffset</span></span>|<span data-ttu-id="202b3-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="202b3-141">The date and time the policy was created.</span></span> <span data-ttu-id="202b3-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="202b3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="202b3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="202b3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="202b3-144">DateTimeOffset</span></span>|<span data-ttu-id="202b3-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="202b3-145">Last time the policy was modified.</span></span> <span data-ttu-id="202b3-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="202b3-147">id</span><span class="sxs-lookup"><span data-stu-id="202b3-147">id</span></span>|<span data-ttu-id="202b3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="202b3-148">String</span></span>|<span data-ttu-id="202b3-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="202b3-149">Key of the entity.</span></span> <span data-ttu-id="202b3-150">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="202b3-151">version</span><span class="sxs-lookup"><span data-stu-id="202b3-151">version</span></span>|<span data-ttu-id="202b3-152">String</span><span class="sxs-lookup"><span data-stu-id="202b3-152">String</span></span>|<span data-ttu-id="202b3-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="202b3-153">Version of the entity.</span></span> <span data-ttu-id="202b3-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="202b3-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="202b3-155">customSettings</span></span>|<span data-ttu-id="202b3-156">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="202b3-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="202b3-157">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="202b3-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="202b3-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="202b3-158">deployedAppCount</span></span>|<span data-ttu-id="202b3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="202b3-159">Int32</span></span>|<span data-ttu-id="202b3-160">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="202b3-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="202b3-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="202b3-161">isAssigned</span></span>|<span data-ttu-id="202b3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="202b3-162">Boolean</span></span>|<span data-ttu-id="202b3-163">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="202b3-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="202b3-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="202b3-164">Response</span></span>
<span data-ttu-id="202b3-165">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="202b3-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="202b3-166">Пример</span><span class="sxs-lookup"><span data-stu-id="202b3-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="202b3-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="202b3-167">Request</span></span>
<span data-ttu-id="202b3-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="202b3-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="202b3-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="202b3-169">Response</span></span>
<span data-ttu-id="202b3-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="202b3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



