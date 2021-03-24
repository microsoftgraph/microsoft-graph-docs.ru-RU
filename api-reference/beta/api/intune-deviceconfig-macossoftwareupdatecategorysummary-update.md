---
title: Обновление macOSSoftwareUpdateCategorySummary
description: Обновление свойств объекта macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92a8f014f94b3639a41ace8d7b40ba30e5a06aa6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131227"
---
# <a name="update-macossoftwareupdatecategorysummary"></a><span data-ttu-id="be09d-103">Обновление macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="be09d-103">Update macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="be09d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be09d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be09d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be09d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be09d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be09d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be09d-107">Обновление свойств объекта [macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="be09d-107">Update the properties of a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be09d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be09d-108">Prerequisites</span></span>
<span data-ttu-id="be09d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be09d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be09d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be09d-111">Permission type</span></span>|<span data-ttu-id="be09d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be09d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be09d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be09d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be09d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be09d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be09d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be09d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be09d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be09d-116">Not supported.</span></span>|
|<span data-ttu-id="be09d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="be09d-117">Application</span></span>|<span data-ttu-id="be09d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be09d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be09d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be09d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="be09d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be09d-120">Request headers</span></span>
|<span data-ttu-id="be09d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be09d-121">Header</span></span>|<span data-ttu-id="be09d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be09d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be09d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be09d-123">Authorization</span></span>|<span data-ttu-id="be09d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be09d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be09d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be09d-125">Accept</span></span>|<span data-ttu-id="be09d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be09d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be09d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be09d-127">Request body</span></span>
<span data-ttu-id="be09d-128">В теле запроса поставляем представление JSON для [объекта macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="be09d-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

<span data-ttu-id="be09d-129">В следующей таблице показаны свойства, необходимые при создании [macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="be09d-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).</span></span>

|<span data-ttu-id="be09d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="be09d-130">Property</span></span>|<span data-ttu-id="be09d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be09d-131">Type</span></span>|<span data-ttu-id="be09d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be09d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be09d-133">id</span><span class="sxs-lookup"><span data-stu-id="be09d-133">id</span></span>|<span data-ttu-id="be09d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="be09d-134">String</span></span>|<span data-ttu-id="be09d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be09d-135">Key of the entity.</span></span>|
|<span data-ttu-id="be09d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="be09d-136">displayName</span></span>|<span data-ttu-id="be09d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="be09d-137">String</span></span>|<span data-ttu-id="be09d-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="be09d-138">The name of the report</span></span>|
|<span data-ttu-id="be09d-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="be09d-139">deviceId</span></span>|<span data-ttu-id="be09d-140">String</span><span class="sxs-lookup"><span data-stu-id="be09d-140">String</span></span>|<span data-ttu-id="be09d-141">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="be09d-141">The device ID.</span></span>|
|<span data-ttu-id="be09d-142">userId</span><span class="sxs-lookup"><span data-stu-id="be09d-142">userId</span></span>|<span data-ttu-id="be09d-143">String</span><span class="sxs-lookup"><span data-stu-id="be09d-143">String</span></span>|<span data-ttu-id="be09d-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="be09d-144">The user ID.</span></span>|
|<span data-ttu-id="be09d-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="be09d-145">updateCategory</span></span>|[<span data-ttu-id="be09d-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="be09d-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="be09d-147">Тип обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="be09d-147">Software update type.</span></span> <span data-ttu-id="be09d-148">Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="be09d-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="be09d-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="be09d-149">successfulUpdateCount</span></span>|<span data-ttu-id="be09d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="be09d-150">Int32</span></span>|<span data-ttu-id="be09d-151">Количество успешных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="be09d-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="be09d-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="be09d-152">failedUpdateCount</span></span>|<span data-ttu-id="be09d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="be09d-153">Int32</span></span>|<span data-ttu-id="be09d-154">Количество сбойных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="be09d-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="be09d-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="be09d-155">totalUpdateCount</span></span>|<span data-ttu-id="be09d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="be09d-156">Int32</span></span>|<span data-ttu-id="be09d-157">Количество обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="be09d-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="be09d-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="be09d-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="be09d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be09d-159">DateTimeOffset</span></span>|<span data-ttu-id="be09d-160">Последняя дата обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="be09d-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="be09d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="be09d-161">Response</span></span>
<span data-ttu-id="be09d-162">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="be09d-162">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be09d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="be09d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="be09d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="be09d-164">Request</span></span>
<span data-ttu-id="be09d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be09d-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="be09d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="be09d-166">Response</span></span>
<span data-ttu-id="be09d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be09d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




