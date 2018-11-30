---
title: Обновление объекта targetedManagedAppConfiguration
description: Обновление свойств объекта targetedManagedAppConfiguration.
ms.openlocfilehash: 097665b53250c90bbe553d72b2e82dabac6a11ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079910"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="caa3a-103">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="caa3a-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="caa3a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="caa3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="caa3a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caa3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="caa3a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="caa3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caa3a-107">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="caa3a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="caa3a-108">Prerequisites</span></span>
<span data-ttu-id="caa3a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caa3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caa3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caa3a-111">Permission type</span></span>|<span data-ttu-id="caa3a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="caa3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caa3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caa3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="caa3a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caa3a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="caa3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caa3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caa3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caa3a-116">Not supported.</span></span>|
|<span data-ttu-id="caa3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caa3a-117">Application</span></span>|<span data-ttu-id="caa3a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caa3a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caa3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caa3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="caa3a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caa3a-120">Request headers</span></span>
|<span data-ttu-id="caa3a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="caa3a-121">Header</span></span>|<span data-ttu-id="caa3a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="caa3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caa3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="caa3a-123">Authorization</span></span>|<span data-ttu-id="caa3a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="caa3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caa3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="caa3a-125">Accept</span></span>|<span data-ttu-id="caa3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="caa3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caa3a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="caa3a-127">Request body</span></span>
<span data-ttu-id="caa3a-128">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caa3a-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="caa3a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="caa3a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="caa3a-130">Property</span></span>|<span data-ttu-id="caa3a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="caa3a-131">Type</span></span>|<span data-ttu-id="caa3a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="caa3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caa3a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="caa3a-133">displayName</span></span>|<span data-ttu-id="caa3a-134">String</span><span class="sxs-lookup"><span data-stu-id="caa3a-134">String</span></span>|<span data-ttu-id="caa3a-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="caa3a-135">Policy display name.</span></span> <span data-ttu-id="caa3a-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="caa3a-137">описание</span><span class="sxs-lookup"><span data-stu-id="caa3a-137">description</span></span>|<span data-ttu-id="caa3a-138">String</span><span class="sxs-lookup"><span data-stu-id="caa3a-138">String</span></span>|<span data-ttu-id="caa3a-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="caa3a-139">The policy's description.</span></span> <span data-ttu-id="caa3a-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="caa3a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caa3a-141">createdDateTime</span></span>|<span data-ttu-id="caa3a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa3a-142">DateTimeOffset</span></span>|<span data-ttu-id="caa3a-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="caa3a-143">The date and time the policy was created.</span></span> <span data-ttu-id="caa3a-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="caa3a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caa3a-145">lastModifiedDateTime</span></span>|<span data-ttu-id="caa3a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa3a-146">DateTimeOffset</span></span>|<span data-ttu-id="caa3a-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="caa3a-147">Last time the policy was modified.</span></span> <span data-ttu-id="caa3a-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="caa3a-149">id</span><span class="sxs-lookup"><span data-stu-id="caa3a-149">id</span></span>|<span data-ttu-id="caa3a-150">String</span><span class="sxs-lookup"><span data-stu-id="caa3a-150">String</span></span>|<span data-ttu-id="caa3a-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="caa3a-151">Key of the entity.</span></span> <span data-ttu-id="caa3a-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="caa3a-153">version</span><span class="sxs-lookup"><span data-stu-id="caa3a-153">version</span></span>|<span data-ttu-id="caa3a-154">String</span><span class="sxs-lookup"><span data-stu-id="caa3a-154">String</span></span>|<span data-ttu-id="caa3a-155">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="caa3a-155">Version of the entity.</span></span> <span data-ttu-id="caa3a-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="caa3a-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="caa3a-157">customSettings</span></span>|<span data-ttu-id="caa3a-158">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="caa3a-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="caa3a-159">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa3a-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="caa3a-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="caa3a-160">deployedAppCount</span></span>|<span data-ttu-id="caa3a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="caa3a-161">Int32</span></span>|<span data-ttu-id="caa3a-162">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="caa3a-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="caa3a-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="caa3a-163">isAssigned</span></span>|<span data-ttu-id="caa3a-164">Логический</span><span class="sxs-lookup"><span data-stu-id="caa3a-164">Boolean</span></span>|<span data-ttu-id="caa3a-165">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="caa3a-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="caa3a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="caa3a-166">Response</span></span>
<span data-ttu-id="caa3a-167">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="caa3a-167">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caa3a-168">Пример</span><span class="sxs-lookup"><span data-stu-id="caa3a-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="caa3a-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="caa3a-169">Request</span></span>
<span data-ttu-id="caa3a-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caa3a-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 382

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="caa3a-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="caa3a-171">Response</span></span>
<span data-ttu-id="caa3a-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="caa3a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





