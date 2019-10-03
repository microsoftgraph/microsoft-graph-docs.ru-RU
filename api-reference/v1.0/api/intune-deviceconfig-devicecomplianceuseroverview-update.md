---
title: Обновление объекта deviceComplianceUserOverview
description: Обновление свойств объекта deviceComplianceUserOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bfe38ef55ef5155555f48154937d5940736176c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368920"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="f80dd-103">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f80dd-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="f80dd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f80dd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f80dd-105">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f80dd-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f80dd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f80dd-106">Prerequisites</span></span>
<span data-ttu-id="f80dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f80dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f80dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f80dd-109">Permission type</span></span>|<span data-ttu-id="f80dd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f80dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f80dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f80dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f80dd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f80dd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f80dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f80dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f80dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f80dd-114">Not supported.</span></span>|
|<span data-ttu-id="f80dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f80dd-115">Application</span></span>|<span data-ttu-id="f80dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f80dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f80dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f80dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f80dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f80dd-118">Request headers</span></span>
|<span data-ttu-id="f80dd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f80dd-119">Header</span></span>|<span data-ttu-id="f80dd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f80dd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f80dd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f80dd-121">Authorization</span></span>|<span data-ttu-id="f80dd-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f80dd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f80dd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f80dd-123">Accept</span></span>|<span data-ttu-id="f80dd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f80dd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f80dd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f80dd-125">Request body</span></span>
<span data-ttu-id="f80dd-126">В тексте запроса добавьте представление объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f80dd-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="f80dd-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f80dd-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="f80dd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f80dd-128">Property</span></span>|<span data-ttu-id="f80dd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f80dd-129">Type</span></span>|<span data-ttu-id="f80dd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f80dd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f80dd-131">id</span><span class="sxs-lookup"><span data-stu-id="f80dd-131">id</span></span>|<span data-ttu-id="f80dd-132">String</span><span class="sxs-lookup"><span data-stu-id="f80dd-132">String</span></span>|<span data-ttu-id="f80dd-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f80dd-133">Key of the entity.</span></span>|
|<span data-ttu-id="f80dd-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f80dd-134">pendingCount</span></span>|<span data-ttu-id="f80dd-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f80dd-135">Int32</span></span>|<span data-ttu-id="f80dd-136">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="f80dd-136">Number of pending Users</span></span>|
|<span data-ttu-id="f80dd-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f80dd-137">notApplicableCount</span></span>|<span data-ttu-id="f80dd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f80dd-138">Int32</span></span>|<span data-ttu-id="f80dd-139">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="f80dd-139">Number of not applicable users</span></span>|
|<span data-ttu-id="f80dd-140">successCount</span><span class="sxs-lookup"><span data-stu-id="f80dd-140">successCount</span></span>|<span data-ttu-id="f80dd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f80dd-141">Int32</span></span>|<span data-ttu-id="f80dd-142">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f80dd-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="f80dd-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="f80dd-143">errorCount</span></span>|<span data-ttu-id="f80dd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f80dd-144">Int32</span></span>|<span data-ttu-id="f80dd-145">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f80dd-145">Number of error Users</span></span>|
|<span data-ttu-id="f80dd-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="f80dd-146">failedCount</span></span>|<span data-ttu-id="f80dd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f80dd-147">Int32</span></span>|<span data-ttu-id="f80dd-148">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="f80dd-148">Number of failed Users</span></span>|
|<span data-ttu-id="f80dd-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f80dd-149">lastUpdateDateTime</span></span>|<span data-ttu-id="f80dd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f80dd-150">DateTimeOffset</span></span>|<span data-ttu-id="f80dd-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="f80dd-151">Last update time</span></span>|
|<span data-ttu-id="f80dd-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f80dd-152">configurationVersion</span></span>|<span data-ttu-id="f80dd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f80dd-153">Int32</span></span>|<span data-ttu-id="f80dd-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="f80dd-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f80dd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f80dd-155">Response</span></span>
<span data-ttu-id="f80dd-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f80dd-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f80dd-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f80dd-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="f80dd-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f80dd-158">Request</span></span>
<span data-ttu-id="f80dd-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f80dd-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f80dd-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f80dd-160">Response</span></span>
<span data-ttu-id="f80dd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f80dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




