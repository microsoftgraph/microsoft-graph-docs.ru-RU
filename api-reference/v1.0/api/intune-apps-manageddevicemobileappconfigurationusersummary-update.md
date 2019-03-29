---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc12a1322dadc4cfafd28b64ec35002ece2ee34e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977900"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="cdeb7-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="cdeb7-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="cdeb7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdeb7-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="cdeb7-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdeb7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cdeb7-106">Prerequisites</span></span>
<span data-ttu-id="cdeb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdeb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdeb7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdeb7-109">Permission type</span></span>|<span data-ttu-id="cdeb7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdeb7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdeb7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdeb7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdeb7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdeb7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cdeb7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdeb7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdeb7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-114">Not supported.</span></span>|
|<span data-ttu-id="cdeb7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdeb7-115">Application</span></span>|<span data-ttu-id="cdeb7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdeb7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdeb7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="cdeb7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdeb7-118">Request headers</span></span>
|<span data-ttu-id="cdeb7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdeb7-119">Header</span></span>|<span data-ttu-id="cdeb7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cdeb7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdeb7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdeb7-121">Authorization</span></span>|<span data-ttu-id="cdeb7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdeb7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cdeb7-123">Accept</span></span>|<span data-ttu-id="cdeb7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdeb7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdeb7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdeb7-125">Request body</span></span>
<span data-ttu-id="cdeb7-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="cdeb7-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="cdeb7-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="cdeb7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdeb7-128">Property</span></span>|<span data-ttu-id="cdeb7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cdeb7-129">Type</span></span>|<span data-ttu-id="cdeb7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cdeb7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdeb7-131">id</span><span class="sxs-lookup"><span data-stu-id="cdeb7-131">id</span></span>|<span data-ttu-id="cdeb7-132">String</span><span class="sxs-lookup"><span data-stu-id="cdeb7-132">String</span></span>|<span data-ttu-id="cdeb7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-133">Key of the entity.</span></span>|
|<span data-ttu-id="cdeb7-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="cdeb7-134">pendingCount</span></span>|<span data-ttu-id="cdeb7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cdeb7-135">Int32</span></span>|<span data-ttu-id="cdeb7-136">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-136">Number of pending Users</span></span>|
|<span data-ttu-id="cdeb7-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cdeb7-137">notApplicableCount</span></span>|<span data-ttu-id="cdeb7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cdeb7-138">Int32</span></span>|<span data-ttu-id="cdeb7-139">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="cdeb7-139">Number of not applicable users</span></span>|
|<span data-ttu-id="cdeb7-140">successCount</span><span class="sxs-lookup"><span data-stu-id="cdeb7-140">successCount</span></span>|<span data-ttu-id="cdeb7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="cdeb7-141">Int32</span></span>|<span data-ttu-id="cdeb7-142">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="cdeb7-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="cdeb7-143">errorCount</span></span>|<span data-ttu-id="cdeb7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cdeb7-144">Int32</span></span>|<span data-ttu-id="cdeb7-145">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-145">Number of error Users</span></span>|
|<span data-ttu-id="cdeb7-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="cdeb7-146">failedCount</span></span>|<span data-ttu-id="cdeb7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cdeb7-147">Int32</span></span>|<span data-ttu-id="cdeb7-148">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-148">Number of failed Users</span></span>|
|<span data-ttu-id="cdeb7-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cdeb7-149">lastUpdateDateTime</span></span>|<span data-ttu-id="cdeb7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdeb7-150">DateTimeOffset</span></span>|<span data-ttu-id="cdeb7-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-151">Last update time</span></span>|
|<span data-ttu-id="cdeb7-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="cdeb7-152">configurationVersion</span></span>|<span data-ttu-id="cdeb7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cdeb7-153">Int32</span></span>|<span data-ttu-id="cdeb7-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="cdeb7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdeb7-155">Response</span></span>
<span data-ttu-id="cdeb7-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdeb7-157">Пример</span><span class="sxs-lookup"><span data-stu-id="cdeb7-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdeb7-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdeb7-158">Request</span></span>
<span data-ttu-id="cdeb7-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cdeb7-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdeb7-160">Response</span></span>
<span data-ttu-id="cdeb7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdeb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



