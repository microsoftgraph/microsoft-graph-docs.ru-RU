---
title: Обновление Девицеманажементинтентусерстатесуммари
description: Обновление свойств объекта Девицеманажементинтентусерстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fad8264139d0a5df5b66b6e4b18f3050dd38704
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470723"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="1a63b-103">Обновление Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="1a63b-103">Update deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="1a63b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a63b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a63b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a63b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a63b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a63b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a63b-107">Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1a63b-107">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a63b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1a63b-108">Prerequisites</span></span>
<span data-ttu-id="1a63b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a63b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a63b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a63b-111">Permission type</span></span>|<span data-ttu-id="1a63b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a63b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a63b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a63b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a63b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a63b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a63b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a63b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a63b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a63b-116">Not supported.</span></span>|
|<span data-ttu-id="1a63b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a63b-117">Application</span></span>|<span data-ttu-id="1a63b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a63b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a63b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a63b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="1a63b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a63b-120">Request headers</span></span>
|<span data-ttu-id="1a63b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a63b-121">Header</span></span>|<span data-ttu-id="1a63b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1a63b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a63b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a63b-123">Authorization</span></span>|<span data-ttu-id="1a63b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a63b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a63b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a63b-125">Accept</span></span>|<span data-ttu-id="1a63b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a63b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a63b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a63b-127">Request body</span></span>
<span data-ttu-id="1a63b-128">В тексте запроса добавьте представление объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a63b-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="1a63b-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1a63b-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="1a63b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a63b-130">Property</span></span>|<span data-ttu-id="1a63b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a63b-131">Type</span></span>|<span data-ttu-id="1a63b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a63b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a63b-133">id</span><span class="sxs-lookup"><span data-stu-id="1a63b-133">id</span></span>|<span data-ttu-id="1a63b-134">String</span><span class="sxs-lookup"><span data-stu-id="1a63b-134">String</span></span>|<span data-ttu-id="1a63b-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="1a63b-135">The ID</span></span>|
|<span data-ttu-id="1a63b-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1a63b-136">conflictCount</span></span>|<span data-ttu-id="1a63b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1a63b-137">Int32</span></span>|<span data-ttu-id="1a63b-138">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="1a63b-138">Number of users in conflict</span></span>|
|<span data-ttu-id="1a63b-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="1a63b-139">errorCount</span></span>|<span data-ttu-id="1a63b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1a63b-140">Int32</span></span>|<span data-ttu-id="1a63b-141">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="1a63b-141">Number of error users</span></span>|
|<span data-ttu-id="1a63b-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="1a63b-142">failedCount</span></span>|<span data-ttu-id="1a63b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1a63b-143">Int32</span></span>|<span data-ttu-id="1a63b-144">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="1a63b-144">Number of failed users</span></span>|
|<span data-ttu-id="1a63b-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1a63b-145">notApplicableCount</span></span>|<span data-ttu-id="1a63b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1a63b-146">Int32</span></span>|<span data-ttu-id="1a63b-147">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="1a63b-147">Number of not applicable users</span></span>|
|<span data-ttu-id="1a63b-148">successCount</span><span class="sxs-lookup"><span data-stu-id="1a63b-148">successCount</span></span>|<span data-ttu-id="1a63b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1a63b-149">Int32</span></span>|<span data-ttu-id="1a63b-150">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="1a63b-150">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="1a63b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a63b-151">Response</span></span>
<span data-ttu-id="1a63b-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a63b-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a63b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="1a63b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a63b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a63b-154">Request</span></span>
<span data-ttu-id="1a63b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a63b-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a63b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a63b-156">Response</span></span>
<span data-ttu-id="1a63b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a63b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





