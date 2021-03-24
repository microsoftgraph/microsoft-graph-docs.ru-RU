---
title: Создание securityBaselineCategoryStateSummary
description: Создайте новый объект securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11fc148bcc4c25f36f315b7c15df2d0266b28845
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136575"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="08971-103">Создание securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="08971-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="08971-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08971-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08971-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08971-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08971-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08971-107">Создайте новый [объект securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08971-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08971-108">Prerequisites</span></span>
<span data-ttu-id="08971-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08971-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08971-111">Permission type</span></span>|<span data-ttu-id="08971-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08971-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08971-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08971-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08971-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08971-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08971-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08971-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08971-116">Not supported.</span></span>|
|<span data-ttu-id="08971-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="08971-117">Application</span></span>|<span data-ttu-id="08971-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08971-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08971-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08971-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="08971-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08971-120">Request headers</span></span>
|<span data-ttu-id="08971-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08971-121">Header</span></span>|<span data-ttu-id="08971-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08971-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08971-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08971-123">Authorization</span></span>|<span data-ttu-id="08971-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08971-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08971-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08971-125">Accept</span></span>|<span data-ttu-id="08971-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08971-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08971-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08971-127">Request body</span></span>
<span data-ttu-id="08971-128">В теле запроса укажи представление JSON для объекта securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="08971-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="08971-129">В следующей таблице показаны свойства, необходимые при создании securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="08971-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="08971-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08971-130">Property</span></span>|<span data-ttu-id="08971-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08971-131">Type</span></span>|<span data-ttu-id="08971-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08971-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08971-133">id</span><span class="sxs-lookup"><span data-stu-id="08971-133">id</span></span>|<span data-ttu-id="08971-134">Строка</span><span class="sxs-lookup"><span data-stu-id="08971-134">String</span></span>|<span data-ttu-id="08971-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="08971-135">Unique identifier of the entity.</span></span> <span data-ttu-id="08971-136">Унаследованный от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="08971-137">secureCount</span></span>|<span data-ttu-id="08971-138">Int32</span><span class="sxs-lookup"><span data-stu-id="08971-138">Int32</span></span>|<span data-ttu-id="08971-139">Количество защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="08971-140">notSecureCount</span></span>|<span data-ttu-id="08971-141">Int32</span><span class="sxs-lookup"><span data-stu-id="08971-141">Int32</span></span>|<span data-ttu-id="08971-142">Количество не защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="08971-143">unknownCount</span></span>|<span data-ttu-id="08971-144">Int32</span><span class="sxs-lookup"><span data-stu-id="08971-144">Int32</span></span>|<span data-ttu-id="08971-145">Количество неизвестных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="08971-146">errorCount</span></span>|<span data-ttu-id="08971-147">Int32</span><span class="sxs-lookup"><span data-stu-id="08971-147">Int32</span></span>|<span data-ttu-id="08971-148">Количество устройств с ошибками, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="08971-149">conflictCount</span></span>|<span data-ttu-id="08971-150">Int32</span><span class="sxs-lookup"><span data-stu-id="08971-150">Int32</span></span>|<span data-ttu-id="08971-151">Количество конфликтных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="08971-152">notApplicableCount</span></span>|<span data-ttu-id="08971-153">Int32</span><span class="sxs-lookup"><span data-stu-id="08971-153">Int32</span></span>|<span data-ttu-id="08971-154">Количество не применимых устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08971-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="08971-155">displayName</span><span class="sxs-lookup"><span data-stu-id="08971-155">displayName</span></span>|<span data-ttu-id="08971-156">Строка</span><span class="sxs-lookup"><span data-stu-id="08971-156">String</span></span>|<span data-ttu-id="08971-157">Имя категории</span><span class="sxs-lookup"><span data-stu-id="08971-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="08971-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="08971-158">Response</span></span>
<span data-ttu-id="08971-159">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="08971-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08971-160">Пример</span><span class="sxs-lookup"><span data-stu-id="08971-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="08971-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="08971-161">Request</span></span>
<span data-ttu-id="08971-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08971-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="08971-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="08971-163">Response</span></span>
<span data-ttu-id="08971-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08971-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




