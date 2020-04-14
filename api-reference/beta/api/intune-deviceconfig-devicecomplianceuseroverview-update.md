---
title: Обновление объекта deviceComplianceUserOverview
description: Обновление свойств объекта deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 547caeb6919260e1f83d4eba9da9be01a68130cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433751"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="57474-103">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="57474-103">Update deviceComplianceUserOverview</span></span>

<span data-ttu-id="57474-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57474-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57474-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57474-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57474-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57474-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57474-107">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="57474-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57474-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="57474-108">Prerequisites</span></span>
<span data-ttu-id="57474-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57474-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57474-111">Permission type</span></span>|<span data-ttu-id="57474-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57474-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57474-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57474-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57474-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57474-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57474-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57474-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57474-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57474-116">Not supported.</span></span>|
|<span data-ttu-id="57474-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="57474-117">Application</span></span>|<span data-ttu-id="57474-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57474-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57474-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57474-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="57474-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57474-120">Request headers</span></span>
|<span data-ttu-id="57474-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57474-121">Header</span></span>|<span data-ttu-id="57474-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57474-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57474-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57474-123">Authorization</span></span>|<span data-ttu-id="57474-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57474-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57474-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57474-125">Accept</span></span>|<span data-ttu-id="57474-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57474-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57474-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57474-127">Request body</span></span>
<span data-ttu-id="57474-128">В тексте запроса добавьте представление объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57474-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="57474-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="57474-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="57474-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57474-130">Property</span></span>|<span data-ttu-id="57474-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57474-131">Type</span></span>|<span data-ttu-id="57474-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57474-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57474-133">id</span><span class="sxs-lookup"><span data-stu-id="57474-133">id</span></span>|<span data-ttu-id="57474-134">String</span><span class="sxs-lookup"><span data-stu-id="57474-134">String</span></span>|<span data-ttu-id="57474-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57474-135">Key of the entity.</span></span>|
|<span data-ttu-id="57474-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="57474-136">pendingCount</span></span>|<span data-ttu-id="57474-137">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-137">Int32</span></span>|<span data-ttu-id="57474-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="57474-138">Number of pending Users</span></span>|
|<span data-ttu-id="57474-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="57474-139">notApplicableCount</span></span>|<span data-ttu-id="57474-140">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-140">Int32</span></span>|<span data-ttu-id="57474-141">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="57474-141">Number of not applicable users</span></span>|
|<span data-ttu-id="57474-142">successCount</span><span class="sxs-lookup"><span data-stu-id="57474-142">successCount</span></span>|<span data-ttu-id="57474-143">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-143">Int32</span></span>|<span data-ttu-id="57474-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="57474-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="57474-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="57474-145">errorCount</span></span>|<span data-ttu-id="57474-146">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-146">Int32</span></span>|<span data-ttu-id="57474-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="57474-147">Number of error Users</span></span>|
|<span data-ttu-id="57474-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="57474-148">failedCount</span></span>|<span data-ttu-id="57474-149">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-149">Int32</span></span>|<span data-ttu-id="57474-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="57474-150">Number of failed Users</span></span>|
|<span data-ttu-id="57474-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="57474-151">conflictCount</span></span>|<span data-ttu-id="57474-152">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-152">Int32</span></span>|<span data-ttu-id="57474-153">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="57474-153">Number of users in conflict</span></span>|
|<span data-ttu-id="57474-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="57474-154">lastUpdateDateTime</span></span>|<span data-ttu-id="57474-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57474-155">DateTimeOffset</span></span>|<span data-ttu-id="57474-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="57474-156">Last update time</span></span>|
|<span data-ttu-id="57474-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="57474-157">configurationVersion</span></span>|<span data-ttu-id="57474-158">Int32</span><span class="sxs-lookup"><span data-stu-id="57474-158">Int32</span></span>|<span data-ttu-id="57474-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="57474-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="57474-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="57474-160">Response</span></span>
<span data-ttu-id="57474-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57474-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57474-162">Пример</span><span class="sxs-lookup"><span data-stu-id="57474-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="57474-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="57474-163">Request</span></span>
<span data-ttu-id="57474-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57474-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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

### <a name="response"></a><span data-ttu-id="57474-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="57474-165">Response</span></span>
<span data-ttu-id="57474-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57474-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
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



