---
title: Обновление объекта deviceComplianceUserOverview
description: Обновление свойств объекта deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4f86323dc4406772759df70ab4c05aa201296e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985239"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="a1581-103">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="a1581-103">Update deviceComplianceUserOverview</span></span>

<span data-ttu-id="a1581-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1581-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1581-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1581-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1581-106">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="a1581-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1581-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a1581-107">Prerequisites</span></span>
<span data-ttu-id="a1581-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1581-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1581-110">Permission type</span></span>|<span data-ttu-id="a1581-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1581-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1581-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1581-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1581-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1581-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1581-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1581-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1581-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1581-115">Not supported.</span></span>|
|<span data-ttu-id="a1581-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1581-116">Application</span></span>|<span data-ttu-id="a1581-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1581-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1581-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1581-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="a1581-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1581-119">Request headers</span></span>
|<span data-ttu-id="a1581-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1581-120">Header</span></span>|<span data-ttu-id="a1581-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1581-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1581-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1581-122">Authorization</span></span>|<span data-ttu-id="a1581-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1581-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1581-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1581-124">Accept</span></span>|<span data-ttu-id="a1581-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1581-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1581-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1581-126">Request body</span></span>
<span data-ttu-id="a1581-127">В тексте запроса добавьте представление объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1581-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="a1581-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="a1581-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="a1581-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1581-129">Property</span></span>|<span data-ttu-id="a1581-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1581-130">Type</span></span>|<span data-ttu-id="a1581-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1581-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1581-132">id</span><span class="sxs-lookup"><span data-stu-id="a1581-132">id</span></span>|<span data-ttu-id="a1581-133">String</span><span class="sxs-lookup"><span data-stu-id="a1581-133">String</span></span>|<span data-ttu-id="a1581-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1581-134">Key of the entity.</span></span>|
|<span data-ttu-id="a1581-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a1581-135">pendingCount</span></span>|<span data-ttu-id="a1581-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a1581-136">Int32</span></span>|<span data-ttu-id="a1581-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="a1581-137">Number of pending Users</span></span>|
|<span data-ttu-id="a1581-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a1581-138">notApplicableCount</span></span>|<span data-ttu-id="a1581-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a1581-139">Int32</span></span>|<span data-ttu-id="a1581-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="a1581-140">Number of not applicable users</span></span>|
|<span data-ttu-id="a1581-141">successCount</span><span class="sxs-lookup"><span data-stu-id="a1581-141">successCount</span></span>|<span data-ttu-id="a1581-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a1581-142">Int32</span></span>|<span data-ttu-id="a1581-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="a1581-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="a1581-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="a1581-144">errorCount</span></span>|<span data-ttu-id="a1581-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a1581-145">Int32</span></span>|<span data-ttu-id="a1581-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a1581-146">Number of error Users</span></span>|
|<span data-ttu-id="a1581-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="a1581-147">failedCount</span></span>|<span data-ttu-id="a1581-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a1581-148">Int32</span></span>|<span data-ttu-id="a1581-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="a1581-149">Number of failed Users</span></span>|
|<span data-ttu-id="a1581-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a1581-150">lastUpdateDateTime</span></span>|<span data-ttu-id="a1581-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1581-151">DateTimeOffset</span></span>|<span data-ttu-id="a1581-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="a1581-152">Last update time</span></span>|
|<span data-ttu-id="a1581-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a1581-153">configurationVersion</span></span>|<span data-ttu-id="a1581-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a1581-154">Int32</span></span>|<span data-ttu-id="a1581-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="a1581-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="a1581-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1581-156">Response</span></span>
<span data-ttu-id="a1581-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1581-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1581-158">Пример</span><span class="sxs-lookup"><span data-stu-id="a1581-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1581-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1581-159">Request</span></span>
<span data-ttu-id="a1581-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1581-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="a1581-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1581-161">Response</span></span>
<span data-ttu-id="a1581-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1581-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```









