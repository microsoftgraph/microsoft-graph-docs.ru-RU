---
title: Обновление объекта deviceComplianceUserOverview
description: Обновление свойств объекта deviceComplianceUserOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbc623b65f4e789f2182640fbd6da45bc1b51e24
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340060"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="c392f-103">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="c392f-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="c392f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c392f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c392f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c392f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c392f-106">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="c392f-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c392f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c392f-107">Prerequisites</span></span>
<span data-ttu-id="c392f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c392f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c392f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c392f-110">Permission type</span></span>|<span data-ttu-id="c392f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c392f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c392f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c392f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c392f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c392f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c392f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c392f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c392f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c392f-115">Not supported.</span></span>|
|<span data-ttu-id="c392f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c392f-116">Application</span></span>|<span data-ttu-id="c392f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c392f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c392f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c392f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="c392f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c392f-119">Request headers</span></span>
|<span data-ttu-id="c392f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c392f-120">Header</span></span>|<span data-ttu-id="c392f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c392f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c392f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c392f-122">Authorization</span></span>|<span data-ttu-id="c392f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c392f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c392f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c392f-124">Accept</span></span>|<span data-ttu-id="c392f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c392f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c392f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c392f-126">Request body</span></span>
<span data-ttu-id="c392f-127">В тексте запроса добавьте представление объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c392f-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="c392f-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="c392f-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="c392f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c392f-129">Property</span></span>|<span data-ttu-id="c392f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c392f-130">Type</span></span>|<span data-ttu-id="c392f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c392f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c392f-132">id</span><span class="sxs-lookup"><span data-stu-id="c392f-132">id</span></span>|<span data-ttu-id="c392f-133">String</span><span class="sxs-lookup"><span data-stu-id="c392f-133">String</span></span>|<span data-ttu-id="c392f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c392f-134">Key of the entity.</span></span>|
|<span data-ttu-id="c392f-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c392f-135">pendingCount</span></span>|<span data-ttu-id="c392f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-136">Int32</span></span>|<span data-ttu-id="c392f-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="c392f-137">Number of pending Users</span></span>|
|<span data-ttu-id="c392f-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c392f-138">notApplicableCount</span></span>|<span data-ttu-id="c392f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-139">Int32</span></span>|<span data-ttu-id="c392f-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="c392f-140">Number of not applicable users</span></span>|
|<span data-ttu-id="c392f-141">successCount</span><span class="sxs-lookup"><span data-stu-id="c392f-141">successCount</span></span>|<span data-ttu-id="c392f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-142">Int32</span></span>|<span data-ttu-id="c392f-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c392f-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="c392f-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="c392f-144">errorCount</span></span>|<span data-ttu-id="c392f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-145">Int32</span></span>|<span data-ttu-id="c392f-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c392f-146">Number of error Users</span></span>|
|<span data-ttu-id="c392f-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="c392f-147">failedCount</span></span>|<span data-ttu-id="c392f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-148">Int32</span></span>|<span data-ttu-id="c392f-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="c392f-149">Number of failed Users</span></span>|
|<span data-ttu-id="c392f-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c392f-150">conflictCount</span></span>|<span data-ttu-id="c392f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-151">Int32</span></span>|<span data-ttu-id="c392f-152">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="c392f-152">Number of users in conflict</span></span>|
|<span data-ttu-id="c392f-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c392f-153">lastUpdateDateTime</span></span>|<span data-ttu-id="c392f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c392f-154">DateTimeOffset</span></span>|<span data-ttu-id="c392f-155">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="c392f-155">Last update time</span></span>|
|<span data-ttu-id="c392f-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c392f-156">configurationVersion</span></span>|<span data-ttu-id="c392f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c392f-157">Int32</span></span>|<span data-ttu-id="c392f-158">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="c392f-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="c392f-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="c392f-159">Response</span></span>
<span data-ttu-id="c392f-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c392f-160">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c392f-161">Пример</span><span class="sxs-lookup"><span data-stu-id="c392f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="c392f-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c392f-162">Request</span></span>
<span data-ttu-id="c392f-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c392f-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c392f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c392f-164">Response</span></span>
<span data-ttu-id="c392f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c392f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






