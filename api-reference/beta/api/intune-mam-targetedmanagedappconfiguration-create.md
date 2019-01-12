---
title: Создание targetedManagedAppConfiguration
description: Создание объекта targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34737ff9d9ae1314cdd667e72fd2c3393bcf0991
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970166"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="bbafe-103">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bbafe-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="bbafe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bbafe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbafe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbafe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbafe-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bbafe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbafe-107">Создание объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbafe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bbafe-108">Prerequisites</span></span>
<span data-ttu-id="bbafe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbafe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbafe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbafe-111">Permission type</span></span>|<span data-ttu-id="bbafe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbafe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbafe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbafe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbafe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbafe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bbafe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbafe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbafe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbafe-116">Not supported.</span></span>|
|<span data-ttu-id="bbafe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbafe-117">Application</span></span>|<span data-ttu-id="bbafe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbafe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbafe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbafe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bbafe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbafe-120">Request headers</span></span>
|<span data-ttu-id="bbafe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbafe-121">Header</span></span>|<span data-ttu-id="bbafe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bbafe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbafe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbafe-123">Authorization</span></span>|<span data-ttu-id="bbafe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bbafe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbafe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bbafe-125">Accept</span></span>|<span data-ttu-id="bbafe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbafe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbafe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbafe-127">Request body</span></span>
<span data-ttu-id="bbafe-128">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbafe-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="bbafe-129">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bbafe-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="bbafe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbafe-130">Property</span></span>|<span data-ttu-id="bbafe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bbafe-131">Type</span></span>|<span data-ttu-id="bbafe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bbafe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbafe-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bbafe-133">displayName</span></span>|<span data-ttu-id="bbafe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bbafe-134">String</span></span>|<span data-ttu-id="bbafe-135">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="bbafe-135">Policy display name.</span></span> <span data-ttu-id="bbafe-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bbafe-137">описание</span><span class="sxs-lookup"><span data-stu-id="bbafe-137">description</span></span>|<span data-ttu-id="bbafe-138">Строка</span><span class="sxs-lookup"><span data-stu-id="bbafe-138">String</span></span>|<span data-ttu-id="bbafe-139">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="bbafe-139">The policy's description.</span></span> <span data-ttu-id="bbafe-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bbafe-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbafe-141">createdDateTime</span></span>|<span data-ttu-id="bbafe-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbafe-142">DateTimeOffset</span></span>|<span data-ttu-id="bbafe-143">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="bbafe-143">The date and time the policy was created.</span></span> <span data-ttu-id="bbafe-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bbafe-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbafe-145">lastModifiedDateTime</span></span>|<span data-ttu-id="bbafe-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbafe-146">DateTimeOffset</span></span>|<span data-ttu-id="bbafe-147">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bbafe-147">Last time the policy was modified.</span></span> <span data-ttu-id="bbafe-148">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bbafe-149">id</span><span class="sxs-lookup"><span data-stu-id="bbafe-149">id</span></span>|<span data-ttu-id="bbafe-150">Строка</span><span class="sxs-lookup"><span data-stu-id="bbafe-150">String</span></span>|<span data-ttu-id="bbafe-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bbafe-151">Key of the entity.</span></span> <span data-ttu-id="bbafe-152">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bbafe-153">version</span><span class="sxs-lookup"><span data-stu-id="bbafe-153">version</span></span>|<span data-ttu-id="bbafe-154">Строка</span><span class="sxs-lookup"><span data-stu-id="bbafe-154">String</span></span>|<span data-ttu-id="bbafe-155">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bbafe-155">Version of the entity.</span></span> <span data-ttu-id="bbafe-156">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="bbafe-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="bbafe-157">customSettings</span></span>|<span data-ttu-id="bbafe-158">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bbafe-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bbafe-159">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bbafe-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="bbafe-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="bbafe-160">deployedAppCount</span></span>|<span data-ttu-id="bbafe-161">Int32</span><span class="sxs-lookup"><span data-stu-id="bbafe-161">Int32</span></span>|<span data-ttu-id="bbafe-162">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="bbafe-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="bbafe-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bbafe-163">isAssigned</span></span>|<span data-ttu-id="bbafe-164">Логический</span><span class="sxs-lookup"><span data-stu-id="bbafe-164">Boolean</span></span>|<span data-ttu-id="bbafe-165">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="bbafe-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="bbafe-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbafe-166">Response</span></span>
<span data-ttu-id="bbafe-167">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bbafe-167">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbafe-168">Пример</span><span class="sxs-lookup"><span data-stu-id="bbafe-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbafe-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbafe-169">Request</span></span>
<span data-ttu-id="bbafe-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbafe-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bbafe-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbafe-171">Response</span></span>
<span data-ttu-id="bbafe-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bbafe-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





