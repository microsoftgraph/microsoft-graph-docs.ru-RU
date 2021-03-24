---
title: Обновление securityBaselineCategoryStateSummary
description: Обновление свойств объекта securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af9b11acf7d5bbf7fe4a4aafd517a8b589abf23e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132004"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="a4e89-103">Обновление securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="a4e89-103">Update securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="a4e89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4e89-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4e89-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4e89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4e89-107">Обновление свойств объекта [securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-107">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4e89-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4e89-108">Prerequisites</span></span>
<span data-ttu-id="a4e89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e89-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4e89-111">Permission type</span></span>|<span data-ttu-id="a4e89-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4e89-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4e89-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4e89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4e89-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e89-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4e89-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4e89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4e89-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e89-116">Not supported.</span></span>|
|<span data-ttu-id="a4e89-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4e89-117">Application</span></span>|<span data-ttu-id="a4e89-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e89-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4e89-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4e89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a4e89-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4e89-120">Request headers</span></span>
|<span data-ttu-id="a4e89-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4e89-121">Header</span></span>|<span data-ttu-id="a4e89-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4e89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4e89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4e89-123">Authorization</span></span>|<span data-ttu-id="a4e89-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4e89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4e89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4e89-125">Accept</span></span>|<span data-ttu-id="a4e89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4e89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4e89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4e89-127">Request body</span></span>
<span data-ttu-id="a4e89-128">В теле запроса укажи представление JSON для объекта [securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-128">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="a4e89-129">В следующей таблице показаны свойства, необходимые при создании [securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-129">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="a4e89-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4e89-130">Property</span></span>|<span data-ttu-id="a4e89-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e89-131">Type</span></span>|<span data-ttu-id="a4e89-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4e89-133">id</span><span class="sxs-lookup"><span data-stu-id="a4e89-133">id</span></span>|<span data-ttu-id="a4e89-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a4e89-134">String</span></span>|<span data-ttu-id="a4e89-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="a4e89-135">Unique identifier of the entity.</span></span> <span data-ttu-id="a4e89-136">Унаследованный от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="a4e89-137">secureCount</span></span>|<span data-ttu-id="a4e89-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e89-138">Int32</span></span>|<span data-ttu-id="a4e89-139">Количество защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="a4e89-140">notSecureCount</span></span>|<span data-ttu-id="a4e89-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e89-141">Int32</span></span>|<span data-ttu-id="a4e89-142">Количество не защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a4e89-143">unknownCount</span></span>|<span data-ttu-id="a4e89-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e89-144">Int32</span></span>|<span data-ttu-id="a4e89-145">Количество неизвестных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="a4e89-146">errorCount</span></span>|<span data-ttu-id="a4e89-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e89-147">Int32</span></span>|<span data-ttu-id="a4e89-148">Количество устройств с ошибками, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a4e89-149">conflictCount</span></span>|<span data-ttu-id="a4e89-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e89-150">Int32</span></span>|<span data-ttu-id="a4e89-151">Количество конфликтных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a4e89-152">notApplicableCount</span></span>|<span data-ttu-id="a4e89-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e89-153">Int32</span></span>|<span data-ttu-id="a4e89-154">Количество не применимых устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4e89-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a4e89-155">displayName</span><span class="sxs-lookup"><span data-stu-id="a4e89-155">displayName</span></span>|<span data-ttu-id="a4e89-156">Строка</span><span class="sxs-lookup"><span data-stu-id="a4e89-156">String</span></span>|<span data-ttu-id="a4e89-157">Имя категории</span><span class="sxs-lookup"><span data-stu-id="a4e89-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="a4e89-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4e89-158">Response</span></span>
<span data-ttu-id="a4e89-159">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4e89-159">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4e89-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a4e89-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4e89-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4e89-161">Request</span></span>
<span data-ttu-id="a4e89-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4e89-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a4e89-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4e89-163">Response</span></span>
<span data-ttu-id="a4e89-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4e89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```




