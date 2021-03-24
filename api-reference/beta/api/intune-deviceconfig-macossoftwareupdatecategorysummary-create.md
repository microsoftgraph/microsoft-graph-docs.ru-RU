---
title: Создание macOSSoftwareUpdateCategorySummary
description: Создайте новый объект macOSSoftwareUpdateCategorySummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc47fac234f046d69235af431db9d75dc1093e40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129715"
---
# <a name="create-macossoftwareupdatecategorysummary"></a><span data-ttu-id="89bbb-103">Создание macOSSoftwareUpdateCategorySummary</span><span class="sxs-lookup"><span data-stu-id="89bbb-103">Create macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="89bbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89bbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89bbb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89bbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89bbb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89bbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89bbb-107">Создайте новый [объект macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)</span><span class="sxs-lookup"><span data-stu-id="89bbb-107">Create a new [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89bbb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89bbb-108">Prerequisites</span></span>
<span data-ttu-id="89bbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89bbb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89bbb-111">Permission type</span></span>|<span data-ttu-id="89bbb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89bbb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89bbb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89bbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89bbb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89bbb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89bbb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89bbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89bbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89bbb-116">Not supported.</span></span>|
|<span data-ttu-id="89bbb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="89bbb-117">Application</span></span>|<span data-ttu-id="89bbb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89bbb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89bbb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89bbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a><span data-ttu-id="89bbb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89bbb-120">Request headers</span></span>
|<span data-ttu-id="89bbb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89bbb-121">Header</span></span>|<span data-ttu-id="89bbb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89bbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89bbb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89bbb-123">Authorization</span></span>|<span data-ttu-id="89bbb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89bbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89bbb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89bbb-125">Accept</span></span>|<span data-ttu-id="89bbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89bbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89bbb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89bbb-127">Request body</span></span>
<span data-ttu-id="89bbb-128">В теле запроса поставляем представление JSON для объекта macOSSoftwareUpdateCategorySummary.</span><span class="sxs-lookup"><span data-stu-id="89bbb-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateCategorySummary object.</span></span>

<span data-ttu-id="89bbb-129">В следующей таблице показаны свойства, необходимые при создании macOSSoftwareUpdateCategorySummary.</span><span class="sxs-lookup"><span data-stu-id="89bbb-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateCategorySummary.</span></span>

|<span data-ttu-id="89bbb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="89bbb-130">Property</span></span>|<span data-ttu-id="89bbb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="89bbb-131">Type</span></span>|<span data-ttu-id="89bbb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="89bbb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89bbb-133">id</span><span class="sxs-lookup"><span data-stu-id="89bbb-133">id</span></span>|<span data-ttu-id="89bbb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="89bbb-134">String</span></span>|<span data-ttu-id="89bbb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89bbb-135">Key of the entity.</span></span>|
|<span data-ttu-id="89bbb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="89bbb-136">displayName</span></span>|<span data-ttu-id="89bbb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="89bbb-137">String</span></span>|<span data-ttu-id="89bbb-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="89bbb-138">The name of the report</span></span>|
|<span data-ttu-id="89bbb-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="89bbb-139">deviceId</span></span>|<span data-ttu-id="89bbb-140">String</span><span class="sxs-lookup"><span data-stu-id="89bbb-140">String</span></span>|<span data-ttu-id="89bbb-141">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="89bbb-141">The device ID.</span></span>|
|<span data-ttu-id="89bbb-142">userId</span><span class="sxs-lookup"><span data-stu-id="89bbb-142">userId</span></span>|<span data-ttu-id="89bbb-143">String</span><span class="sxs-lookup"><span data-stu-id="89bbb-143">String</span></span>|<span data-ttu-id="89bbb-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="89bbb-144">The user ID.</span></span>|
|<span data-ttu-id="89bbb-145">updateCategory</span><span class="sxs-lookup"><span data-stu-id="89bbb-145">updateCategory</span></span>|[<span data-ttu-id="89bbb-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="89bbb-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="89bbb-147">Тип обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="89bbb-147">Software update type.</span></span> <span data-ttu-id="89bbb-148">Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="89bbb-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="89bbb-149">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="89bbb-149">successfulUpdateCount</span></span>|<span data-ttu-id="89bbb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="89bbb-150">Int32</span></span>|<span data-ttu-id="89bbb-151">Количество успешных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="89bbb-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="89bbb-152">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="89bbb-152">failedUpdateCount</span></span>|<span data-ttu-id="89bbb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="89bbb-153">Int32</span></span>|<span data-ttu-id="89bbb-154">Количество сбойных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="89bbb-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="89bbb-155">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="89bbb-155">totalUpdateCount</span></span>|<span data-ttu-id="89bbb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="89bbb-156">Int32</span></span>|<span data-ttu-id="89bbb-157">Количество обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="89bbb-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="89bbb-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="89bbb-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="89bbb-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89bbb-159">DateTimeOffset</span></span>|<span data-ttu-id="89bbb-160">Последняя дата обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="89bbb-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="89bbb-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="89bbb-161">Response</span></span>
<span data-ttu-id="89bbb-162">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89bbb-162">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89bbb-163">Пример</span><span class="sxs-lookup"><span data-stu-id="89bbb-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="89bbb-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="89bbb-164">Request</span></span>
<span data-ttu-id="89bbb-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89bbb-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
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

### <a name="response"></a><span data-ttu-id="89bbb-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="89bbb-166">Response</span></span>
<span data-ttu-id="89bbb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89bbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




