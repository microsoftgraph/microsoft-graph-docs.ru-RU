---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
ms.openlocfilehash: b5b639bf517867ca23634c9af788ccbf91396b67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333910"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="b29eb-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b29eb-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="b29eb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b29eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b29eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b29eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b29eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b29eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b29eb-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b29eb-107">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b29eb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b29eb-108">Prerequisites</span></span>
<span data-ttu-id="b29eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b29eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b29eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b29eb-111">Permission type</span></span>|<span data-ttu-id="b29eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b29eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b29eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b29eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b29eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b29eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b29eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b29eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b29eb-116">Not supported.</span></span>|
|<span data-ttu-id="b29eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b29eb-117">Application</span></span>|<span data-ttu-id="b29eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b29eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b29eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b29eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="b29eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b29eb-120">Request headers</span></span>
|<span data-ttu-id="b29eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b29eb-121">Header</span></span>|<span data-ttu-id="b29eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b29eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b29eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b29eb-123">Authorization</span></span>|<span data-ttu-id="b29eb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b29eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b29eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b29eb-125">Accept</span></span>|<span data-ttu-id="b29eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b29eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b29eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b29eb-127">Request body</span></span>
<span data-ttu-id="b29eb-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b29eb-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="b29eb-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b29eb-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="b29eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b29eb-130">Property</span></span>|<span data-ttu-id="b29eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b29eb-131">Type</span></span>|<span data-ttu-id="b29eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b29eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b29eb-133">id</span><span class="sxs-lookup"><span data-stu-id="b29eb-133">id</span></span>|<span data-ttu-id="b29eb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b29eb-134">String</span></span>|<span data-ttu-id="b29eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b29eb-135">Key of the entity.</span></span>|
|<span data-ttu-id="b29eb-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b29eb-136">pendingCount</span></span>|<span data-ttu-id="b29eb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-137">Int32</span></span>|<span data-ttu-id="b29eb-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="b29eb-138">Number of pending Users</span></span>|
|<span data-ttu-id="b29eb-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b29eb-139">notApplicableCount</span></span>|<span data-ttu-id="b29eb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-140">Int32</span></span>|<span data-ttu-id="b29eb-141">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="b29eb-141">Number of not applicable users</span></span>|
|<span data-ttu-id="b29eb-142">successCount</span><span class="sxs-lookup"><span data-stu-id="b29eb-142">successCount</span></span>|<span data-ttu-id="b29eb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-143">Int32</span></span>|<span data-ttu-id="b29eb-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="b29eb-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="b29eb-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="b29eb-145">errorCount</span></span>|<span data-ttu-id="b29eb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-146">Int32</span></span>|<span data-ttu-id="b29eb-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b29eb-147">Number of error Users</span></span>|
|<span data-ttu-id="b29eb-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="b29eb-148">failedCount</span></span>|<span data-ttu-id="b29eb-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-149">Int32</span></span>|<span data-ttu-id="b29eb-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b29eb-150">Number of failed Users</span></span>|
|<span data-ttu-id="b29eb-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b29eb-151">conflictCount</span></span>|<span data-ttu-id="b29eb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-152">Int32</span></span>|<span data-ttu-id="b29eb-153">Количество пользователей в конфликта</span><span class="sxs-lookup"><span data-stu-id="b29eb-153">Number of users in conflict</span></span>|
|<span data-ttu-id="b29eb-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b29eb-154">lastUpdateDateTime</span></span>|<span data-ttu-id="b29eb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b29eb-155">DateTimeOffset</span></span>|<span data-ttu-id="b29eb-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="b29eb-156">Last update time</span></span>|
|<span data-ttu-id="b29eb-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b29eb-157">configurationVersion</span></span>|<span data-ttu-id="b29eb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b29eb-158">Int32</span></span>|<span data-ttu-id="b29eb-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="b29eb-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="b29eb-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b29eb-160">Response</span></span>
<span data-ttu-id="b29eb-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b29eb-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b29eb-162">Пример</span><span class="sxs-lookup"><span data-stu-id="b29eb-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="b29eb-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b29eb-163">Request</span></span>
<span data-ttu-id="b29eb-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b29eb-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 236

{
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

### <a name="response"></a><span data-ttu-id="b29eb-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="b29eb-165">Response</span></span>
<span data-ttu-id="b29eb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b29eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





