---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3151bfc6427d778db3d13053357b239d8870a35a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961429"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="1a670-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1a670-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="1a670-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a670-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a670-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="1a670-106">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a670-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a670-107">Prerequisites</span></span>
<span data-ttu-id="1a670-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a670-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a670-110">Permission type</span></span>|<span data-ttu-id="1a670-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a670-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a670-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a670-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a670-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a670-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a670-115">Not supported.</span></span>|
|<span data-ttu-id="1a670-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a670-116">Application</span></span>|<span data-ttu-id="1a670-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a670-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a670-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="1a670-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a670-119">Request headers</span></span>
|<span data-ttu-id="1a670-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a670-120">Header</span></span>|<span data-ttu-id="1a670-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a670-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a670-122">Authorization</span></span>|<span data-ttu-id="1a670-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a670-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a670-124">Accept</span></span>|<span data-ttu-id="1a670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a670-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a670-126">Request body</span></span>
<span data-ttu-id="1a670-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a670-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="1a670-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="1a670-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="1a670-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a670-129">Property</span></span>|<span data-ttu-id="1a670-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a670-130">Type</span></span>|<span data-ttu-id="1a670-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a670-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a670-132">id</span><span class="sxs-lookup"><span data-stu-id="1a670-132">id</span></span>|<span data-ttu-id="1a670-133">String</span><span class="sxs-lookup"><span data-stu-id="1a670-133">String</span></span>|<span data-ttu-id="1a670-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1a670-134">Key of the entity.</span></span>|
|<span data-ttu-id="1a670-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1a670-135">pendingCount</span></span>|<span data-ttu-id="1a670-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-136">Int32</span></span>|<span data-ttu-id="1a670-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="1a670-137">Number of pending Users</span></span>|
|<span data-ttu-id="1a670-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1a670-138">notApplicableCount</span></span>|<span data-ttu-id="1a670-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-139">Int32</span></span>|<span data-ttu-id="1a670-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="1a670-140">Number of not applicable users</span></span>|
|<span data-ttu-id="1a670-141">successCount</span><span class="sxs-lookup"><span data-stu-id="1a670-141">successCount</span></span>|<span data-ttu-id="1a670-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-142">Int32</span></span>|<span data-ttu-id="1a670-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1a670-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="1a670-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="1a670-144">errorCount</span></span>|<span data-ttu-id="1a670-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-145">Int32</span></span>|<span data-ttu-id="1a670-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1a670-146">Number of error Users</span></span>|
|<span data-ttu-id="1a670-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="1a670-147">failedCount</span></span>|<span data-ttu-id="1a670-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-148">Int32</span></span>|<span data-ttu-id="1a670-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="1a670-149">Number of failed Users</span></span>|
|<span data-ttu-id="1a670-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1a670-150">conflictCount</span></span>|<span data-ttu-id="1a670-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-151">Int32</span></span>|<span data-ttu-id="1a670-152">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="1a670-152">Number of users in conflict</span></span>|
|<span data-ttu-id="1a670-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1a670-153">lastUpdateDateTime</span></span>|<span data-ttu-id="1a670-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a670-154">DateTimeOffset</span></span>|<span data-ttu-id="1a670-155">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="1a670-155">Last update time</span></span>|
|<span data-ttu-id="1a670-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1a670-156">configurationVersion</span></span>|<span data-ttu-id="1a670-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1a670-157">Int32</span></span>|<span data-ttu-id="1a670-158">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="1a670-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="1a670-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a670-159">Response</span></span>
<span data-ttu-id="1a670-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a670-160">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a670-161">Пример</span><span class="sxs-lookup"><span data-stu-id="1a670-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a670-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a670-162">Request</span></span>
<span data-ttu-id="1a670-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a670-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a670-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a670-164">Response</span></span>
<span data-ttu-id="1a670-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a670-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





