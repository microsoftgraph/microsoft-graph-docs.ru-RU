---
title: Обновление Девицеманажементинтентусерстатесуммари
description: Обновление свойств объекта Девицеманажементинтентусерстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5a1f0ec0d51b9537d3147d4fdcc58220456662f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734408"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="deb0e-103">Обновление Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="deb0e-103">Update deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="deb0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="deb0e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="deb0e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="deb0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deb0e-107">Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="deb0e-107">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deb0e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="deb0e-108">Prerequisites</span></span>
<span data-ttu-id="deb0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb0e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb0e-111">Permission type</span></span>|<span data-ttu-id="deb0e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb0e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="deb0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="deb0e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb0e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb0e-116">Not supported.</span></span>|
|<span data-ttu-id="deb0e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deb0e-117">Application</span></span>|<span data-ttu-id="deb0e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb0e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb0e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="deb0e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="deb0e-120">Request headers</span></span>
|<span data-ttu-id="deb0e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="deb0e-121">Header</span></span>|<span data-ttu-id="deb0e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="deb0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deb0e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="deb0e-123">Authorization</span></span>|<span data-ttu-id="deb0e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deb0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="deb0e-125">Accept</span></span>|<span data-ttu-id="deb0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="deb0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb0e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="deb0e-127">Request body</span></span>
<span data-ttu-id="deb0e-128">В тексте запроса добавьте представление объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="deb0e-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="deb0e-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="deb0e-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="deb0e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb0e-130">Property</span></span>|<span data-ttu-id="deb0e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="deb0e-131">Type</span></span>|<span data-ttu-id="deb0e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="deb0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb0e-133">id</span><span class="sxs-lookup"><span data-stu-id="deb0e-133">id</span></span>|<span data-ttu-id="deb0e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="deb0e-134">String</span></span>|<span data-ttu-id="deb0e-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="deb0e-135">The ID</span></span>|
|<span data-ttu-id="deb0e-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="deb0e-136">conflictCount</span></span>|<span data-ttu-id="deb0e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="deb0e-137">Int32</span></span>|<span data-ttu-id="deb0e-138">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="deb0e-138">Number of users in conflict</span></span>|
|<span data-ttu-id="deb0e-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="deb0e-139">errorCount</span></span>|<span data-ttu-id="deb0e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="deb0e-140">Int32</span></span>|<span data-ttu-id="deb0e-141">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="deb0e-141">Number of error users</span></span>|
|<span data-ttu-id="deb0e-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="deb0e-142">failedCount</span></span>|<span data-ttu-id="deb0e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="deb0e-143">Int32</span></span>|<span data-ttu-id="deb0e-144">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="deb0e-144">Number of failed users</span></span>|
|<span data-ttu-id="deb0e-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="deb0e-145">notApplicableCount</span></span>|<span data-ttu-id="deb0e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="deb0e-146">Int32</span></span>|<span data-ttu-id="deb0e-147">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="deb0e-147">Number of not applicable users</span></span>|
|<span data-ttu-id="deb0e-148">successCount</span><span class="sxs-lookup"><span data-stu-id="deb0e-148">successCount</span></span>|<span data-ttu-id="deb0e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="deb0e-149">Int32</span></span>|<span data-ttu-id="deb0e-150">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="deb0e-150">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="deb0e-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="deb0e-151">Response</span></span>
<span data-ttu-id="deb0e-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="deb0e-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deb0e-153">Пример</span><span class="sxs-lookup"><span data-stu-id="deb0e-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="deb0e-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb0e-154">Request</span></span>
<span data-ttu-id="deb0e-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb0e-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="deb0e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb0e-156">Response</span></span>
<span data-ttu-id="deb0e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="deb0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





