---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90aadd0cf51843bad7888777c2a8de7a75beb228
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013922"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="8e9fb-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="8e9fb-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="8e9fb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e9fb-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e9fb-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e9fb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e9fb-106">Prerequisites</span></span>
<span data-ttu-id="8e9fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e9fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e9fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e9fb-109">Permission type</span></span>|<span data-ttu-id="8e9fb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e9fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e9fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e9fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e9fb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e9fb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e9fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e9fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e9fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-114">Not supported.</span></span>|
|<span data-ttu-id="8e9fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e9fb-115">Application</span></span>|<span data-ttu-id="8e9fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e9fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e9fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="8e9fb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e9fb-118">Request headers</span></span>
|<span data-ttu-id="8e9fb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e9fb-119">Header</span></span>|<span data-ttu-id="8e9fb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8e9fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e9fb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e9fb-121">Authorization</span></span>|<span data-ttu-id="8e9fb-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e9fb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8e9fb-123">Accept</span></span>|<span data-ttu-id="8e9fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e9fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e9fb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e9fb-125">Request body</span></span>
<span data-ttu-id="8e9fb-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="8e9fb-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e9fb-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="8e9fb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e9fb-128">Property</span></span>|<span data-ttu-id="8e9fb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8e9fb-129">Type</span></span>|<span data-ttu-id="8e9fb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8e9fb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e9fb-131">id</span><span class="sxs-lookup"><span data-stu-id="8e9fb-131">id</span></span>|<span data-ttu-id="8e9fb-132">String</span><span class="sxs-lookup"><span data-stu-id="8e9fb-132">String</span></span>|<span data-ttu-id="8e9fb-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-133">Key of the entity.</span></span>|
|<span data-ttu-id="8e9fb-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="8e9fb-134">pendingCount</span></span>|<span data-ttu-id="8e9fb-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9fb-135">Int32</span></span>|<span data-ttu-id="8e9fb-136">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-136">Number of pending Users</span></span>|
|<span data-ttu-id="8e9fb-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8e9fb-137">notApplicableCount</span></span>|<span data-ttu-id="8e9fb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9fb-138">Int32</span></span>|<span data-ttu-id="8e9fb-139">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="8e9fb-139">Number of not applicable users</span></span>|
|<span data-ttu-id="8e9fb-140">successCount</span><span class="sxs-lookup"><span data-stu-id="8e9fb-140">successCount</span></span>|<span data-ttu-id="8e9fb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9fb-141">Int32</span></span>|<span data-ttu-id="8e9fb-142">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="8e9fb-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="8e9fb-143">errorCount</span></span>|<span data-ttu-id="8e9fb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9fb-144">Int32</span></span>|<span data-ttu-id="8e9fb-145">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-145">Number of error Users</span></span>|
|<span data-ttu-id="8e9fb-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="8e9fb-146">failedCount</span></span>|<span data-ttu-id="8e9fb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9fb-147">Int32</span></span>|<span data-ttu-id="8e9fb-148">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-148">Number of failed Users</span></span>|
|<span data-ttu-id="8e9fb-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9fb-149">lastUpdateDateTime</span></span>|<span data-ttu-id="8e9fb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9fb-150">DateTimeOffset</span></span>|<span data-ttu-id="8e9fb-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-151">Last update time</span></span>|
|<span data-ttu-id="8e9fb-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="8e9fb-152">configurationVersion</span></span>|<span data-ttu-id="8e9fb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9fb-153">Int32</span></span>|<span data-ttu-id="8e9fb-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="8e9fb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e9fb-155">Response</span></span>
<span data-ttu-id="8e9fb-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9fb-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8e9fb-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e9fb-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e9fb-158">Request</span></span>
<span data-ttu-id="8e9fb-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="8e9fb-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e9fb-160">Response</span></span>
<span data-ttu-id="8e9fb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e9fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



