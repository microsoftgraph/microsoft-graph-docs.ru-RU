---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73e0d4577af7e32c482421ad4b76ae4549caa46e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936775"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="1b3a1-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1b3a1-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="1b3a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b3a1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b3a1-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="1b3a1-106">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b3a1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b3a1-107">Prerequisites</span></span>
<span data-ttu-id="1b3a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b3a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b3a1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b3a1-110">Permission type</span></span>|<span data-ttu-id="1b3a1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b3a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b3a1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b3a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b3a1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b3a1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b3a1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b3a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b3a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-115">Not supported.</span></span>|
|<span data-ttu-id="1b3a1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b3a1-116">Application</span></span>|<span data-ttu-id="1b3a1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b3a1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b3a1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b3a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="1b3a1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1b3a1-119">Request headers</span></span>
|<span data-ttu-id="1b3a1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b3a1-120">Header</span></span>|<span data-ttu-id="1b3a1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b3a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b3a1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b3a1-122">Authorization</span></span>|<span data-ttu-id="1b3a1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b3a1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b3a1-124">Accept</span></span>|<span data-ttu-id="1b3a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b3a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b3a1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b3a1-126">Request body</span></span>
<span data-ttu-id="1b3a1-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="1b3a1-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="1b3a1-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="1b3a1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b3a1-129">Property</span></span>|<span data-ttu-id="1b3a1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b3a1-130">Type</span></span>|<span data-ttu-id="1b3a1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b3a1-132">id</span><span class="sxs-lookup"><span data-stu-id="1b3a1-132">id</span></span>|<span data-ttu-id="1b3a1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1b3a1-133">String</span></span>|<span data-ttu-id="1b3a1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-134">Key of the entity.</span></span>|
|<span data-ttu-id="1b3a1-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1b3a1-135">pendingCount</span></span>|<span data-ttu-id="1b3a1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-136">Int32</span></span>|<span data-ttu-id="1b3a1-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-137">Number of pending Users</span></span>|
|<span data-ttu-id="1b3a1-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1b3a1-138">notApplicableCount</span></span>|<span data-ttu-id="1b3a1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-139">Int32</span></span>|<span data-ttu-id="1b3a1-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="1b3a1-140">Number of not applicable users</span></span>|
|<span data-ttu-id="1b3a1-141">successCount</span><span class="sxs-lookup"><span data-stu-id="1b3a1-141">successCount</span></span>|<span data-ttu-id="1b3a1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-142">Int32</span></span>|<span data-ttu-id="1b3a1-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="1b3a1-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="1b3a1-144">errorCount</span></span>|<span data-ttu-id="1b3a1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-145">Int32</span></span>|<span data-ttu-id="1b3a1-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-146">Number of error Users</span></span>|
|<span data-ttu-id="1b3a1-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="1b3a1-147">failedCount</span></span>|<span data-ttu-id="1b3a1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-148">Int32</span></span>|<span data-ttu-id="1b3a1-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-149">Number of failed Users</span></span>|
|<span data-ttu-id="1b3a1-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1b3a1-150">conflictCount</span></span>|<span data-ttu-id="1b3a1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-151">Int32</span></span>|<span data-ttu-id="1b3a1-152">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="1b3a1-152">Number of users in conflict</span></span>|
|<span data-ttu-id="1b3a1-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1b3a1-153">lastUpdateDateTime</span></span>|<span data-ttu-id="1b3a1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b3a1-154">DateTimeOffset</span></span>|<span data-ttu-id="1b3a1-155">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-155">Last update time</span></span>|
|<span data-ttu-id="1b3a1-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1b3a1-156">configurationVersion</span></span>|<span data-ttu-id="1b3a1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1b3a1-157">Int32</span></span>|<span data-ttu-id="1b3a1-158">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="1b3a1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b3a1-159">Response</span></span>
<span data-ttu-id="1b3a1-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-160">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b3a1-161">Пример</span><span class="sxs-lookup"><span data-stu-id="1b3a1-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b3a1-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b3a1-162">Request</span></span>
<span data-ttu-id="1b3a1-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b3a1-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b3a1-164">Response</span></span>
<span data-ttu-id="1b3a1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b3a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





