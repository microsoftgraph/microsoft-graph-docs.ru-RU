---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5789ce7e4daca6719fa106159f03157a6a0469a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260951"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="00b53-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="00b53-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="00b53-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00b53-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00b53-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="00b53-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00b53-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00b53-106">Prerequisites</span></span>
<span data-ttu-id="00b53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="00b53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="00b53-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00b53-109">Permission type</span></span>|<span data-ttu-id="00b53-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00b53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00b53-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00b53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00b53-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b53-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00b53-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00b53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00b53-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00b53-114">Not supported.</span></span>|
|<span data-ttu-id="00b53-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00b53-115">Application</span></span>|<span data-ttu-id="00b53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00b53-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00b53-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00b53-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="00b53-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00b53-118">Request headers</span></span>
|<span data-ttu-id="00b53-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00b53-119">Header</span></span>|<span data-ttu-id="00b53-120">Значение</span><span class="sxs-lookup"><span data-stu-id="00b53-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00b53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00b53-121">Authorization</span></span>|<span data-ttu-id="00b53-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00b53-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00b53-123">Accept</span><span class="sxs-lookup"><span data-stu-id="00b53-123">Accept</span></span>|<span data-ttu-id="00b53-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00b53-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00b53-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00b53-125">Request body</span></span>
<span data-ttu-id="00b53-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00b53-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="00b53-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="00b53-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="00b53-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="00b53-128">Property</span></span>|<span data-ttu-id="00b53-129">Тип</span><span class="sxs-lookup"><span data-stu-id="00b53-129">Type</span></span>|<span data-ttu-id="00b53-130">Описание</span><span class="sxs-lookup"><span data-stu-id="00b53-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00b53-131">id</span><span class="sxs-lookup"><span data-stu-id="00b53-131">id</span></span>|<span data-ttu-id="00b53-132">String</span><span class="sxs-lookup"><span data-stu-id="00b53-132">String</span></span>|<span data-ttu-id="00b53-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00b53-133">Key of the entity.</span></span>|
|<span data-ttu-id="00b53-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="00b53-134">pendingCount</span></span>|<span data-ttu-id="00b53-135">Int32</span><span class="sxs-lookup"><span data-stu-id="00b53-135">Int32</span></span>|<span data-ttu-id="00b53-136">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="00b53-136">Number of pending Users</span></span>|
|<span data-ttu-id="00b53-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="00b53-137">notApplicableCount</span></span>|<span data-ttu-id="00b53-138">Int32</span><span class="sxs-lookup"><span data-stu-id="00b53-138">Int32</span></span>|<span data-ttu-id="00b53-139">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="00b53-139">Number of not applicable users</span></span>|
|<span data-ttu-id="00b53-140">successCount</span><span class="sxs-lookup"><span data-stu-id="00b53-140">successCount</span></span>|<span data-ttu-id="00b53-141">Int32</span><span class="sxs-lookup"><span data-stu-id="00b53-141">Int32</span></span>|<span data-ttu-id="00b53-142">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="00b53-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="00b53-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="00b53-143">errorCount</span></span>|<span data-ttu-id="00b53-144">Int32</span><span class="sxs-lookup"><span data-stu-id="00b53-144">Int32</span></span>|<span data-ttu-id="00b53-145">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="00b53-145">Number of error Users</span></span>|
|<span data-ttu-id="00b53-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="00b53-146">failedCount</span></span>|<span data-ttu-id="00b53-147">Int32</span><span class="sxs-lookup"><span data-stu-id="00b53-147">Int32</span></span>|<span data-ttu-id="00b53-148">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="00b53-148">Number of failed Users</span></span>|
|<span data-ttu-id="00b53-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="00b53-149">lastUpdateDateTime</span></span>|<span data-ttu-id="00b53-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00b53-150">DateTimeOffset</span></span>|<span data-ttu-id="00b53-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="00b53-151">Last update time</span></span>|
|<span data-ttu-id="00b53-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="00b53-152">configurationVersion</span></span>|<span data-ttu-id="00b53-153">Int32</span><span class="sxs-lookup"><span data-stu-id="00b53-153">Int32</span></span>|<span data-ttu-id="00b53-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="00b53-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="00b53-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="00b53-155">Response</span></span>
<span data-ttu-id="00b53-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00b53-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00b53-157">Пример</span><span class="sxs-lookup"><span data-stu-id="00b53-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="00b53-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="00b53-158">Request</span></span>
<span data-ttu-id="00b53-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00b53-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00b53-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="00b53-160">Response</span></span>
<span data-ttu-id="00b53-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00b53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



