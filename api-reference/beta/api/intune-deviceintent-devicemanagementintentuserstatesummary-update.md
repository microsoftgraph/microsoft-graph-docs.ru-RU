---
title: Обновление Девицеманажементинтентусерстатесуммари
description: Обновление свойств объекта Девицеманажементинтентусерстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7eb98c9c77c5bc8cecef7994fd2913111bd913fb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915763"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="3c076-103">Обновление Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="3c076-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="3c076-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c076-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c076-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c076-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c076-106">Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3c076-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c076-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c076-107">Prerequisites</span></span>
<span data-ttu-id="3c076-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c076-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c076-110">Permission type</span></span>|<span data-ttu-id="3c076-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c076-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c076-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c076-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c076-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c076-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c076-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c076-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c076-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c076-115">Not supported.</span></span>|
|<span data-ttu-id="3c076-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c076-116">Application</span></span>|<span data-ttu-id="3c076-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c076-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c076-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c076-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3c076-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c076-119">Request headers</span></span>
|<span data-ttu-id="3c076-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c076-120">Header</span></span>|<span data-ttu-id="3c076-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3c076-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c076-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c076-122">Authorization</span></span>|<span data-ttu-id="3c076-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c076-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c076-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3c076-124">Accept</span></span>|<span data-ttu-id="3c076-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c076-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c076-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c076-126">Request body</span></span>
<span data-ttu-id="3c076-127">В тексте запроса добавьте представление объекта [Девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c076-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="3c076-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3c076-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="3c076-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c076-129">Property</span></span>|<span data-ttu-id="3c076-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3c076-130">Type</span></span>|<span data-ttu-id="3c076-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3c076-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c076-132">id</span><span class="sxs-lookup"><span data-stu-id="3c076-132">id</span></span>|<span data-ttu-id="3c076-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3c076-133">String</span></span>|<span data-ttu-id="3c076-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3c076-134">The ID</span></span>|
|<span data-ttu-id="3c076-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="3c076-135">conflictCount</span></span>|<span data-ttu-id="3c076-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3c076-136">Int32</span></span>|<span data-ttu-id="3c076-137">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="3c076-137">Number of users in conflict</span></span>|
|<span data-ttu-id="3c076-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="3c076-138">errorCount</span></span>|<span data-ttu-id="3c076-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3c076-139">Int32</span></span>|<span data-ttu-id="3c076-140">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="3c076-140">Number of error users</span></span>|
|<span data-ttu-id="3c076-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="3c076-141">failedCount</span></span>|<span data-ttu-id="3c076-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3c076-142">Int32</span></span>|<span data-ttu-id="3c076-143">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="3c076-143">Number of failed users</span></span>|
|<span data-ttu-id="3c076-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="3c076-144">notApplicableCount</span></span>|<span data-ttu-id="3c076-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3c076-145">Int32</span></span>|<span data-ttu-id="3c076-146">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="3c076-146">Number of not applicable users</span></span>|
|<span data-ttu-id="3c076-147">successCount</span><span class="sxs-lookup"><span data-stu-id="3c076-147">successCount</span></span>|<span data-ttu-id="3c076-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3c076-148">Int32</span></span>|<span data-ttu-id="3c076-149">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="3c076-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="3c076-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c076-150">Response</span></span>
<span data-ttu-id="3c076-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c076-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c076-152">Пример</span><span class="sxs-lookup"><span data-stu-id="3c076-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c076-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c076-153">Request</span></span>
<span data-ttu-id="3c076-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c076-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
Content-type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="3c076-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c076-155">Response</span></span>
<span data-ttu-id="3c076-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c076-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "be567e02-7e02-be56-027e-56be027e56be",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```




