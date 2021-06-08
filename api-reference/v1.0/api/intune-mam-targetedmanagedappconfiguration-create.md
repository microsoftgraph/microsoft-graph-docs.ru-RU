---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b0745e3ed0ee59502508ef03f2bc1b6559312e2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760344"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="bae87-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bae87-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="bae87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bae87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bae87-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bae87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bae87-106">Создание объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bae87-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bae87-107">Prerequisites</span></span>
<span data-ttu-id="bae87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bae87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae87-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bae87-110">Permission type</span></span>|<span data-ttu-id="bae87-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bae87-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bae87-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bae87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bae87-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae87-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bae87-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bae87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bae87-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bae87-115">Not supported.</span></span>|
|<span data-ttu-id="bae87-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bae87-116">Application</span></span>|<span data-ttu-id="bae87-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae87-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bae87-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bae87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bae87-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bae87-119">Request headers</span></span>
|<span data-ttu-id="bae87-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bae87-120">Header</span></span>|<span data-ttu-id="bae87-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bae87-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bae87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae87-122">Authorization</span></span>|<span data-ttu-id="bae87-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bae87-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bae87-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bae87-124">Accept</span></span>|<span data-ttu-id="bae87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bae87-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bae87-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bae87-126">Request body</span></span>
<span data-ttu-id="bae87-127">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bae87-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="bae87-128">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bae87-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="bae87-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bae87-129">Property</span></span>|<span data-ttu-id="bae87-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bae87-130">Type</span></span>|<span data-ttu-id="bae87-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bae87-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bae87-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bae87-132">displayName</span></span>|<span data-ttu-id="bae87-133">String</span><span class="sxs-lookup"><span data-stu-id="bae87-133">String</span></span>|<span data-ttu-id="bae87-134">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="bae87-134">Policy display name.</span></span> <span data-ttu-id="bae87-135">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bae87-136">description</span><span class="sxs-lookup"><span data-stu-id="bae87-136">description</span></span>|<span data-ttu-id="bae87-137">String</span><span class="sxs-lookup"><span data-stu-id="bae87-137">String</span></span>|<span data-ttu-id="bae87-138">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="bae87-138">The policy's description.</span></span> <span data-ttu-id="bae87-139">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bae87-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bae87-140">createdDateTime</span></span>|<span data-ttu-id="bae87-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae87-141">DateTimeOffset</span></span>|<span data-ttu-id="bae87-142">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="bae87-142">The date and time the policy was created.</span></span> <span data-ttu-id="bae87-143">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bae87-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bae87-144">lastModifiedDateTime</span></span>|<span data-ttu-id="bae87-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae87-145">DateTimeOffset</span></span>|<span data-ttu-id="bae87-146">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bae87-146">Last time the policy was modified.</span></span> <span data-ttu-id="bae87-147">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bae87-148">id</span><span class="sxs-lookup"><span data-stu-id="bae87-148">id</span></span>|<span data-ttu-id="bae87-149">String</span><span class="sxs-lookup"><span data-stu-id="bae87-149">String</span></span>|<span data-ttu-id="bae87-150">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bae87-150">Key of the entity.</span></span> <span data-ttu-id="bae87-151">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bae87-152">version</span><span class="sxs-lookup"><span data-stu-id="bae87-152">version</span></span>|<span data-ttu-id="bae87-153">String</span><span class="sxs-lookup"><span data-stu-id="bae87-153">String</span></span>|<span data-ttu-id="bae87-154">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bae87-154">Version of the entity.</span></span> <span data-ttu-id="bae87-155">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bae87-156">customSettings</span><span class="sxs-lookup"><span data-stu-id="bae87-156">customSettings</span></span>|<span data-ttu-id="bae87-157">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bae87-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bae87-158">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bae87-158">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="bae87-159">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="bae87-159">deployedAppCount</span></span>|<span data-ttu-id="bae87-160">Int32</span><span class="sxs-lookup"><span data-stu-id="bae87-160">Int32</span></span>|<span data-ttu-id="bae87-161">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="bae87-161">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="bae87-162">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bae87-162">isAssigned</span></span>|<span data-ttu-id="bae87-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="bae87-163">Boolean</span></span>|<span data-ttu-id="bae87-164">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="bae87-164">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="bae87-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="bae87-165">Response</span></span>
<span data-ttu-id="bae87-166">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bae87-166">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae87-167">Пример</span><span class="sxs-lookup"><span data-stu-id="bae87-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="bae87-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="bae87-168">Request</span></span>
<span data-ttu-id="bae87-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bae87-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
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

### <a name="response"></a><span data-ttu-id="bae87-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="bae87-170">Response</span></span>
<span data-ttu-id="bae87-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bae87-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




