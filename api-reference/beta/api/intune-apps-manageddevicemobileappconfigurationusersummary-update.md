---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d181ccde69b90e62e5add99f025b8ab6125ed536
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974621"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="69eb7-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="69eb7-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="69eb7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69eb7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69eb7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69eb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69eb7-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="69eb7-106">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69eb7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69eb7-107">Prerequisites</span></span>
<span data-ttu-id="69eb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69eb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69eb7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69eb7-110">Permission type</span></span>|<span data-ttu-id="69eb7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69eb7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69eb7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69eb7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69eb7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69eb7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69eb7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69eb7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69eb7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69eb7-115">Not supported.</span></span>|
|<span data-ttu-id="69eb7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69eb7-116">Application</span></span>|<span data-ttu-id="69eb7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69eb7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69eb7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69eb7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="69eb7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69eb7-119">Request headers</span></span>
|<span data-ttu-id="69eb7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69eb7-120">Header</span></span>|<span data-ttu-id="69eb7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69eb7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69eb7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69eb7-122">Authorization</span></span>|<span data-ttu-id="69eb7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69eb7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69eb7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69eb7-124">Accept</span></span>|<span data-ttu-id="69eb7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69eb7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69eb7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69eb7-126">Request body</span></span>
<span data-ttu-id="69eb7-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69eb7-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="69eb7-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="69eb7-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="69eb7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69eb7-129">Property</span></span>|<span data-ttu-id="69eb7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69eb7-130">Type</span></span>|<span data-ttu-id="69eb7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69eb7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69eb7-132">id</span><span class="sxs-lookup"><span data-stu-id="69eb7-132">id</span></span>|<span data-ttu-id="69eb7-133">String</span><span class="sxs-lookup"><span data-stu-id="69eb7-133">String</span></span>|<span data-ttu-id="69eb7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="69eb7-134">Key of the entity.</span></span>|
|<span data-ttu-id="69eb7-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="69eb7-135">pendingCount</span></span>|<span data-ttu-id="69eb7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-136">Int32</span></span>|<span data-ttu-id="69eb7-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="69eb7-137">Number of pending Users</span></span>|
|<span data-ttu-id="69eb7-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="69eb7-138">notApplicableCount</span></span>|<span data-ttu-id="69eb7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-139">Int32</span></span>|<span data-ttu-id="69eb7-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="69eb7-140">Number of not applicable users</span></span>|
|<span data-ttu-id="69eb7-141">successCount</span><span class="sxs-lookup"><span data-stu-id="69eb7-141">successCount</span></span>|<span data-ttu-id="69eb7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-142">Int32</span></span>|<span data-ttu-id="69eb7-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="69eb7-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="69eb7-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="69eb7-144">errorCount</span></span>|<span data-ttu-id="69eb7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-145">Int32</span></span>|<span data-ttu-id="69eb7-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="69eb7-146">Number of error Users</span></span>|
|<span data-ttu-id="69eb7-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="69eb7-147">failedCount</span></span>|<span data-ttu-id="69eb7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-148">Int32</span></span>|<span data-ttu-id="69eb7-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="69eb7-149">Number of failed Users</span></span>|
|<span data-ttu-id="69eb7-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="69eb7-150">conflictCount</span></span>|<span data-ttu-id="69eb7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-151">Int32</span></span>|<span data-ttu-id="69eb7-152">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="69eb7-152">Number of users in conflict</span></span>|
|<span data-ttu-id="69eb7-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="69eb7-153">lastUpdateDateTime</span></span>|<span data-ttu-id="69eb7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69eb7-154">DateTimeOffset</span></span>|<span data-ttu-id="69eb7-155">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="69eb7-155">Last update time</span></span>|
|<span data-ttu-id="69eb7-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="69eb7-156">configurationVersion</span></span>|<span data-ttu-id="69eb7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="69eb7-157">Int32</span></span>|<span data-ttu-id="69eb7-158">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="69eb7-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="69eb7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="69eb7-159">Response</span></span>
<span data-ttu-id="69eb7-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69eb7-160">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69eb7-161">Пример</span><span class="sxs-lookup"><span data-stu-id="69eb7-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="69eb7-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="69eb7-162">Request</span></span>
<span data-ttu-id="69eb7-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69eb7-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69eb7-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="69eb7-164">Response</span></span>
<span data-ttu-id="69eb7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69eb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





