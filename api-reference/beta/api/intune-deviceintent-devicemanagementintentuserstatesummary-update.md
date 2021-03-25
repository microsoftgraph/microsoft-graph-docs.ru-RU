---
title: Обновление deviceManagementIntentUserStateSummary
description: Обновление свойств объекта deviceManagementIntentUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23de4af33eacac6e4eeffe92fff53243fdf63f36
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150803"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="dd543-103">Обновление deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="dd543-103">Update deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="dd543-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd543-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd543-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd543-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd543-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd543-107">Обновление свойств объекта [deviceManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="dd543-107">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd543-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd543-108">Prerequisites</span></span>
<span data-ttu-id="dd543-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd543-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd543-111">Permission type</span></span>|<span data-ttu-id="dd543-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd543-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd543-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd543-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd543-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd543-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd543-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd543-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd543-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd543-116">Not supported.</span></span>|
|<span data-ttu-id="dd543-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd543-117">Application</span></span>|<span data-ttu-id="dd543-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd543-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd543-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd543-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="dd543-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd543-120">Request headers</span></span>
|<span data-ttu-id="dd543-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd543-121">Header</span></span>|<span data-ttu-id="dd543-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd543-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd543-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd543-123">Authorization</span></span>|<span data-ttu-id="dd543-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd543-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd543-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd543-125">Accept</span></span>|<span data-ttu-id="dd543-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd543-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd543-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd543-127">Request body</span></span>
<span data-ttu-id="dd543-128">В корпусе запроса поставляем представление JSON для [объекта deviceManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="dd543-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="dd543-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="dd543-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="dd543-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd543-130">Property</span></span>|<span data-ttu-id="dd543-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd543-131">Type</span></span>|<span data-ttu-id="dd543-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd543-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd543-133">id</span><span class="sxs-lookup"><span data-stu-id="dd543-133">id</span></span>|<span data-ttu-id="dd543-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dd543-134">String</span></span>|<span data-ttu-id="dd543-135">The ID</span><span class="sxs-lookup"><span data-stu-id="dd543-135">The ID</span></span>|
|<span data-ttu-id="dd543-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="dd543-136">conflictCount</span></span>|<span data-ttu-id="dd543-137">Int32</span><span class="sxs-lookup"><span data-stu-id="dd543-137">Int32</span></span>|<span data-ttu-id="dd543-138">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="dd543-138">Number of users in conflict</span></span>|
|<span data-ttu-id="dd543-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="dd543-139">errorCount</span></span>|<span data-ttu-id="dd543-140">Int32</span><span class="sxs-lookup"><span data-stu-id="dd543-140">Int32</span></span>|<span data-ttu-id="dd543-141">Число пользователей ошибок</span><span class="sxs-lookup"><span data-stu-id="dd543-141">Number of error users</span></span>|
|<span data-ttu-id="dd543-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="dd543-142">failedCount</span></span>|<span data-ttu-id="dd543-143">Int32</span><span class="sxs-lookup"><span data-stu-id="dd543-143">Int32</span></span>|<span data-ttu-id="dd543-144">Число сбойных пользователей</span><span class="sxs-lookup"><span data-stu-id="dd543-144">Number of failed users</span></span>|
|<span data-ttu-id="dd543-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="dd543-145">notApplicableCount</span></span>|<span data-ttu-id="dd543-146">Int32</span><span class="sxs-lookup"><span data-stu-id="dd543-146">Int32</span></span>|<span data-ttu-id="dd543-147">Число не применимых пользователей</span><span class="sxs-lookup"><span data-stu-id="dd543-147">Number of not applicable users</span></span>|
|<span data-ttu-id="dd543-148">successCount</span><span class="sxs-lookup"><span data-stu-id="dd543-148">successCount</span></span>|<span data-ttu-id="dd543-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dd543-149">Int32</span></span>|<span data-ttu-id="dd543-150">Число пользователей, успешно успешно</span><span class="sxs-lookup"><span data-stu-id="dd543-150">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="dd543-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd543-151">Response</span></span>
<span data-ttu-id="dd543-152">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd543-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd543-153">Пример</span><span class="sxs-lookup"><span data-stu-id="dd543-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd543-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd543-154">Request</span></span>
<span data-ttu-id="dd543-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd543-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dd543-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd543-156">Response</span></span>
<span data-ttu-id="dd543-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd543-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




