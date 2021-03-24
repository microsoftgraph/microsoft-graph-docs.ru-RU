---
title: Обновление объекта deviceComplianceUserOverview
description: Обновление свойств объекта deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3b723c5adf2149808707d506dc5c62922c5ad8d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128119"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="a4a03-103">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="a4a03-103">Update deviceComplianceUserOverview</span></span>

<span data-ttu-id="a4a03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4a03-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4a03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4a03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4a03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4a03-107">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="a4a03-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4a03-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a4a03-108">Prerequisites</span></span>
<span data-ttu-id="a4a03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4a03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4a03-111">Permission type</span></span>|<span data-ttu-id="a4a03-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4a03-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4a03-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4a03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4a03-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a03-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4a03-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4a03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4a03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4a03-116">Not supported.</span></span>|
|<span data-ttu-id="a4a03-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4a03-117">Application</span></span>|<span data-ttu-id="a4a03-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a03-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4a03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4a03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="a4a03-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4a03-120">Request headers</span></span>
|<span data-ttu-id="a4a03-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4a03-121">Header</span></span>|<span data-ttu-id="a4a03-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4a03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4a03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a03-123">Authorization</span></span>|<span data-ttu-id="a4a03-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4a03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4a03-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4a03-125">Accept</span></span>|<span data-ttu-id="a4a03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4a03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4a03-127">Request body</span></span>
<span data-ttu-id="a4a03-128">В тексте запроса добавьте представление объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4a03-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="a4a03-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="a4a03-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="a4a03-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4a03-130">Property</span></span>|<span data-ttu-id="a4a03-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4a03-131">Type</span></span>|<span data-ttu-id="a4a03-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4a03-133">id</span><span class="sxs-lookup"><span data-stu-id="a4a03-133">id</span></span>|<span data-ttu-id="a4a03-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a4a03-134">String</span></span>|<span data-ttu-id="a4a03-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4a03-135">Key of the entity.</span></span>|
|<span data-ttu-id="a4a03-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a4a03-136">pendingCount</span></span>|<span data-ttu-id="a4a03-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-137">Int32</span></span>|<span data-ttu-id="a4a03-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="a4a03-138">Number of pending Users</span></span>|
|<span data-ttu-id="a4a03-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a4a03-139">notApplicableCount</span></span>|<span data-ttu-id="a4a03-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-140">Int32</span></span>|<span data-ttu-id="a4a03-141">Число не применимых пользователей</span><span class="sxs-lookup"><span data-stu-id="a4a03-141">Number of not applicable users</span></span>|
|<span data-ttu-id="a4a03-142">successCount</span><span class="sxs-lookup"><span data-stu-id="a4a03-142">successCount</span></span>|<span data-ttu-id="a4a03-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-143">Int32</span></span>|<span data-ttu-id="a4a03-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="a4a03-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="a4a03-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="a4a03-145">errorCount</span></span>|<span data-ttu-id="a4a03-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-146">Int32</span></span>|<span data-ttu-id="a4a03-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a4a03-147">Number of error Users</span></span>|
|<span data-ttu-id="a4a03-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="a4a03-148">failedCount</span></span>|<span data-ttu-id="a4a03-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-149">Int32</span></span>|<span data-ttu-id="a4a03-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="a4a03-150">Number of failed Users</span></span>|
|<span data-ttu-id="a4a03-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a4a03-151">conflictCount</span></span>|<span data-ttu-id="a4a03-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-152">Int32</span></span>|<span data-ttu-id="a4a03-153">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="a4a03-153">Number of users in conflict</span></span>|
|<span data-ttu-id="a4a03-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a4a03-154">lastUpdateDateTime</span></span>|<span data-ttu-id="a4a03-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4a03-155">DateTimeOffset</span></span>|<span data-ttu-id="a4a03-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="a4a03-156">Last update time</span></span>|
|<span data-ttu-id="a4a03-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a4a03-157">configurationVersion</span></span>|<span data-ttu-id="a4a03-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a4a03-158">Int32</span></span>|<span data-ttu-id="a4a03-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="a4a03-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="a4a03-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4a03-160">Response</span></span>
<span data-ttu-id="a4a03-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4a03-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a03-162">Пример</span><span class="sxs-lookup"><span data-stu-id="a4a03-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4a03-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4a03-163">Request</span></span>
<span data-ttu-id="a4a03-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4a03-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4a03-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4a03-165">Response</span></span>
<span data-ttu-id="a4a03-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4a03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




