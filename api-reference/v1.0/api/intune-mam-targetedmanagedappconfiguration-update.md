---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e9cf1f31539789109bc7c538c2a318ae8d685e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916105"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="140be-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="140be-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="140be-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="140be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="140be-105">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="140be-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="140be-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="140be-106">Prerequisites</span></span>
<span data-ttu-id="140be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="140be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="140be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="140be-109">Permission type</span></span>|<span data-ttu-id="140be-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="140be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="140be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="140be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="140be-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="140be-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="140be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="140be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="140be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="140be-114">Not supported.</span></span>|
|<span data-ttu-id="140be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="140be-115">Application</span></span>|<span data-ttu-id="140be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="140be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="140be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="140be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="140be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="140be-118">Request headers</span></span>
|<span data-ttu-id="140be-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="140be-119">Header</span></span>|<span data-ttu-id="140be-120">Значение</span><span class="sxs-lookup"><span data-stu-id="140be-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="140be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="140be-121">Authorization</span></span>|<span data-ttu-id="140be-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="140be-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="140be-123">Accept</span><span class="sxs-lookup"><span data-stu-id="140be-123">Accept</span></span>|<span data-ttu-id="140be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="140be-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="140be-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="140be-125">Request body</span></span>
<span data-ttu-id="140be-126">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="140be-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="140be-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="140be-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="140be-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="140be-128">Property</span></span>|<span data-ttu-id="140be-129">Тип</span><span class="sxs-lookup"><span data-stu-id="140be-129">Type</span></span>|<span data-ttu-id="140be-130">Описание</span><span class="sxs-lookup"><span data-stu-id="140be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="140be-131">displayName</span><span class="sxs-lookup"><span data-stu-id="140be-131">displayName</span></span>|<span data-ttu-id="140be-132">String</span><span class="sxs-lookup"><span data-stu-id="140be-132">String</span></span>|<span data-ttu-id="140be-133">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="140be-133">Policy display name.</span></span> <span data-ttu-id="140be-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="140be-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="140be-135">описание</span><span class="sxs-lookup"><span data-stu-id="140be-135">description</span></span>|<span data-ttu-id="140be-136">String</span><span class="sxs-lookup"><span data-stu-id="140be-136">String</span></span>|<span data-ttu-id="140be-137">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="140be-137">The policy's description.</span></span> <span data-ttu-id="140be-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="140be-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="140be-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="140be-139">createdDateTime</span></span>|<span data-ttu-id="140be-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="140be-140">DateTimeOffset</span></span>|<span data-ttu-id="140be-141">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="140be-141">The date and time the policy was created.</span></span> <span data-ttu-id="140be-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="140be-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="140be-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="140be-143">lastModifiedDateTime</span></span>|<span data-ttu-id="140be-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="140be-144">DateTimeOffset</span></span>|<span data-ttu-id="140be-145">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="140be-145">Last time the policy was modified.</span></span> <span data-ttu-id="140be-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="140be-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="140be-147">id</span><span class="sxs-lookup"><span data-stu-id="140be-147">id</span></span>|<span data-ttu-id="140be-148">String</span><span class="sxs-lookup"><span data-stu-id="140be-148">String</span></span>|<span data-ttu-id="140be-149">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="140be-149">Key of the entity.</span></span> <span data-ttu-id="140be-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="140be-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="140be-151">version</span><span class="sxs-lookup"><span data-stu-id="140be-151">version</span></span>|<span data-ttu-id="140be-152">String</span><span class="sxs-lookup"><span data-stu-id="140be-152">String</span></span>|<span data-ttu-id="140be-153">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="140be-153">Version of the entity.</span></span> <span data-ttu-id="140be-154">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="140be-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="140be-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="140be-155">customSettings</span></span>|<span data-ttu-id="140be-156">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="140be-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="140be-157">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="140be-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="140be-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="140be-158">deployedAppCount</span></span>|<span data-ttu-id="140be-159">Int32</span><span class="sxs-lookup"><span data-stu-id="140be-159">Int32</span></span>|<span data-ttu-id="140be-160">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="140be-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="140be-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="140be-161">isAssigned</span></span>|<span data-ttu-id="140be-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="140be-162">Boolean</span></span>|<span data-ttu-id="140be-163">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="140be-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="140be-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="140be-164">Response</span></span>
<span data-ttu-id="140be-165">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="140be-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="140be-166">Пример</span><span class="sxs-lookup"><span data-stu-id="140be-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="140be-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="140be-167">Request</span></span>
<span data-ttu-id="140be-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="140be-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="140be-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="140be-169">Response</span></span>
<span data-ttu-id="140be-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="140be-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



