---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7729480ca5322cbd8bb5d158c800ced30ee2f6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450960"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="a543a-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="a543a-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

<span data-ttu-id="a543a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a543a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a543a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a543a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a543a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a543a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a543a-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="a543a-107">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a543a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a543a-108">Prerequisites</span></span>
<span data-ttu-id="a543a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a543a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a543a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a543a-111">Permission type</span></span>|<span data-ttu-id="a543a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a543a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a543a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a543a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a543a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a543a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a543a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a543a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a543a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a543a-116">Not supported.</span></span>|
|<span data-ttu-id="a543a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a543a-117">Application</span></span>|<span data-ttu-id="a543a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a543a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a543a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a543a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a543a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a543a-120">Request headers</span></span>
|<span data-ttu-id="a543a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a543a-121">Header</span></span>|<span data-ttu-id="a543a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a543a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a543a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a543a-123">Authorization</span></span>|<span data-ttu-id="a543a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a543a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a543a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a543a-125">Accept</span></span>|<span data-ttu-id="a543a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a543a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a543a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a543a-127">Request body</span></span>
<span data-ttu-id="a543a-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a543a-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="a543a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="a543a-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="a543a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a543a-130">Property</span></span>|<span data-ttu-id="a543a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a543a-131">Type</span></span>|<span data-ttu-id="a543a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a543a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a543a-133">id</span><span class="sxs-lookup"><span data-stu-id="a543a-133">id</span></span>|<span data-ttu-id="a543a-134">String</span><span class="sxs-lookup"><span data-stu-id="a543a-134">String</span></span>|<span data-ttu-id="a543a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a543a-135">Key of the entity.</span></span>|
|<span data-ttu-id="a543a-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a543a-136">pendingCount</span></span>|<span data-ttu-id="a543a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-137">Int32</span></span>|<span data-ttu-id="a543a-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="a543a-138">Number of pending Users</span></span>|
|<span data-ttu-id="a543a-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a543a-139">notApplicableCount</span></span>|<span data-ttu-id="a543a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-140">Int32</span></span>|<span data-ttu-id="a543a-141">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="a543a-141">Number of not applicable users</span></span>|
|<span data-ttu-id="a543a-142">successCount</span><span class="sxs-lookup"><span data-stu-id="a543a-142">successCount</span></span>|<span data-ttu-id="a543a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-143">Int32</span></span>|<span data-ttu-id="a543a-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="a543a-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="a543a-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="a543a-145">errorCount</span></span>|<span data-ttu-id="a543a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-146">Int32</span></span>|<span data-ttu-id="a543a-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a543a-147">Number of error Users</span></span>|
|<span data-ttu-id="a543a-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="a543a-148">failedCount</span></span>|<span data-ttu-id="a543a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-149">Int32</span></span>|<span data-ttu-id="a543a-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="a543a-150">Number of failed Users</span></span>|
|<span data-ttu-id="a543a-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a543a-151">conflictCount</span></span>|<span data-ttu-id="a543a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-152">Int32</span></span>|<span data-ttu-id="a543a-153">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="a543a-153">Number of users in conflict</span></span>|
|<span data-ttu-id="a543a-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a543a-154">lastUpdateDateTime</span></span>|<span data-ttu-id="a543a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a543a-155">DateTimeOffset</span></span>|<span data-ttu-id="a543a-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="a543a-156">Last update time</span></span>|
|<span data-ttu-id="a543a-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a543a-157">configurationVersion</span></span>|<span data-ttu-id="a543a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a543a-158">Int32</span></span>|<span data-ttu-id="a543a-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="a543a-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="a543a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a543a-160">Response</span></span>
<span data-ttu-id="a543a-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a543a-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a543a-162">Пример</span><span class="sxs-lookup"><span data-stu-id="a543a-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a543a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="a543a-163">Request</span></span>
<span data-ttu-id="a543a-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a543a-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 321

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="a543a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a543a-165">Response</span></span>
<span data-ttu-id="a543a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a543a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





