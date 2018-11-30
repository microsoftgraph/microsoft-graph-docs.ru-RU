---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
ms.openlocfilehash: d65fed3c202e418133a0d657ac1496ad97b32c07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080934"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="68d79-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="68d79-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="68d79-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="68d79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68d79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68d79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68d79-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68d79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68d79-107">Создание объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68d79-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68d79-108">Prerequisites</span></span>
<span data-ttu-id="68d79-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68d79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68d79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68d79-111">Permission type</span></span>|<span data-ttu-id="68d79-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68d79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68d79-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68d79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68d79-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68d79-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68d79-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68d79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68d79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68d79-116">Not supported.</span></span>|
|<span data-ttu-id="68d79-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68d79-117">Application</span></span>|<span data-ttu-id="68d79-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68d79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68d79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68d79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="68d79-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68d79-120">Request headers</span></span>
|<span data-ttu-id="68d79-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68d79-121">Header</span></span>|<span data-ttu-id="68d79-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68d79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68d79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68d79-123">Authorization</span></span>|<span data-ttu-id="68d79-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="68d79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68d79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68d79-125">Accept</span></span>|<span data-ttu-id="68d79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68d79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68d79-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68d79-127">Request body</span></span>
<span data-ttu-id="68d79-128">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68d79-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="68d79-129">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68d79-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="68d79-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68d79-130">Property</span></span>|<span data-ttu-id="68d79-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68d79-131">Type</span></span>|<span data-ttu-id="68d79-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68d79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68d79-133">displayName</span><span class="sxs-lookup"><span data-stu-id="68d79-133">displayName</span></span>|<span data-ttu-id="68d79-134">String</span><span class="sxs-lookup"><span data-stu-id="68d79-134">String</span></span>|<span data-ttu-id="68d79-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="68d79-135">Policy display name.</span></span> <span data-ttu-id="68d79-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="68d79-137">описание</span><span class="sxs-lookup"><span data-stu-id="68d79-137">description</span></span>|<span data-ttu-id="68d79-138">String</span><span class="sxs-lookup"><span data-stu-id="68d79-138">String</span></span>|<span data-ttu-id="68d79-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="68d79-139">The policy's description.</span></span> <span data-ttu-id="68d79-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="68d79-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68d79-141">createdDateTime</span></span>|<span data-ttu-id="68d79-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68d79-142">DateTimeOffset</span></span>|<span data-ttu-id="68d79-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="68d79-143">The date and time the policy was created.</span></span> <span data-ttu-id="68d79-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="68d79-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68d79-145">lastModifiedDateTime</span></span>|<span data-ttu-id="68d79-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68d79-146">DateTimeOffset</span></span>|<span data-ttu-id="68d79-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="68d79-147">Last time the policy was modified.</span></span> <span data-ttu-id="68d79-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="68d79-149">id</span><span class="sxs-lookup"><span data-stu-id="68d79-149">id</span></span>|<span data-ttu-id="68d79-150">String</span><span class="sxs-lookup"><span data-stu-id="68d79-150">String</span></span>|<span data-ttu-id="68d79-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68d79-151">Key of the entity.</span></span> <span data-ttu-id="68d79-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="68d79-153">version</span><span class="sxs-lookup"><span data-stu-id="68d79-153">version</span></span>|<span data-ttu-id="68d79-154">String</span><span class="sxs-lookup"><span data-stu-id="68d79-154">String</span></span>|<span data-ttu-id="68d79-155">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="68d79-155">Version of the entity.</span></span> <span data-ttu-id="68d79-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="68d79-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="68d79-157">customSettings</span></span>|<span data-ttu-id="68d79-158">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="68d79-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="68d79-159">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68d79-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="68d79-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="68d79-160">deployedAppCount</span></span>|<span data-ttu-id="68d79-161">Int32</span><span class="sxs-lookup"><span data-stu-id="68d79-161">Int32</span></span>|<span data-ttu-id="68d79-162">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="68d79-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="68d79-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="68d79-163">isAssigned</span></span>|<span data-ttu-id="68d79-164">Логический</span><span class="sxs-lookup"><span data-stu-id="68d79-164">Boolean</span></span>|<span data-ttu-id="68d79-165">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="68d79-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="68d79-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="68d79-166">Response</span></span>
<span data-ttu-id="68d79-167">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68d79-167">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68d79-168">Пример</span><span class="sxs-lookup"><span data-stu-id="68d79-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="68d79-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="68d79-169">Request</span></span>
<span data-ttu-id="68d79-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68d79-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="68d79-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="68d79-171">Response</span></span>
<span data-ttu-id="68d79-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="68d79-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





