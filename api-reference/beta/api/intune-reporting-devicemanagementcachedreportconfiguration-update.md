---
title: Обновление deviceManagementCachedReportConfiguration
description: Обновление свойств объекта deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b9304713a7b7d278991f8dd9ea07ecaece8f4bb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123394"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="cf29b-103">Обновление deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf29b-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="cf29b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf29b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf29b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf29b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf29b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf29b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf29b-107">Обновление свойств объекта [deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf29b-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf29b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf29b-108">Prerequisites</span></span>
<span data-ttu-id="cf29b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf29b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf29b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf29b-111">Permission type</span></span>|<span data-ttu-id="cf29b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf29b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf29b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf29b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf29b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf29b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cf29b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf29b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf29b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf29b-116">Not supported.</span></span>|
|<span data-ttu-id="cf29b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf29b-117">Application</span></span>|<span data-ttu-id="cf29b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf29b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf29b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf29b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cf29b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf29b-120">Request headers</span></span>
|<span data-ttu-id="cf29b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf29b-121">Header</span></span>|<span data-ttu-id="cf29b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf29b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf29b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf29b-123">Authorization</span></span>|<span data-ttu-id="cf29b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf29b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf29b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf29b-125">Accept</span></span>|<span data-ttu-id="cf29b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf29b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf29b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf29b-127">Request body</span></span>
<span data-ttu-id="cf29b-128">В теле запроса поставляем представление JSON для [объекта deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf29b-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="cf29b-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf29b-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="cf29b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf29b-130">Property</span></span>|<span data-ttu-id="cf29b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf29b-131">Type</span></span>|<span data-ttu-id="cf29b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf29b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf29b-133">id</span><span class="sxs-lookup"><span data-stu-id="cf29b-133">id</span></span>|<span data-ttu-id="cf29b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cf29b-134">String</span></span>|<span data-ttu-id="cf29b-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="cf29b-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="cf29b-136">reportName</span><span class="sxs-lookup"><span data-stu-id="cf29b-136">reportName</span></span>|<span data-ttu-id="cf29b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cf29b-137">String</span></span>|<span data-ttu-id="cf29b-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="cf29b-138">Name of the report</span></span>|
|<span data-ttu-id="cf29b-139">filter</span><span class="sxs-lookup"><span data-stu-id="cf29b-139">filter</span></span>|<span data-ttu-id="cf29b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="cf29b-140">String</span></span>|<span data-ttu-id="cf29b-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="cf29b-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="cf29b-142">select</span><span class="sxs-lookup"><span data-stu-id="cf29b-142">select</span></span>|<span data-ttu-id="cf29b-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf29b-143">String collection</span></span>|<span data-ttu-id="cf29b-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="cf29b-144">Columns selected from the report</span></span>|
|<span data-ttu-id="cf29b-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="cf29b-145">orderBy</span></span>|<span data-ttu-id="cf29b-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf29b-146">String collection</span></span>|<span data-ttu-id="cf29b-147">Порядок столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="cf29b-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="cf29b-148">метаданные</span><span class="sxs-lookup"><span data-stu-id="cf29b-148">metadata</span></span>|<span data-ttu-id="cf29b-149">Строка</span><span class="sxs-lookup"><span data-stu-id="cf29b-149">String</span></span>|<span data-ttu-id="cf29b-150">Метаданные, управляемые вызывателями, связанные с отчетом</span><span class="sxs-lookup"><span data-stu-id="cf29b-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="cf29b-151">status</span><span class="sxs-lookup"><span data-stu-id="cf29b-151">status</span></span>|[<span data-ttu-id="cf29b-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="cf29b-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="cf29b-153">Состояние кэшного отчета.</span><span class="sxs-lookup"><span data-stu-id="cf29b-153">Status of the cached report.</span></span> <span data-ttu-id="cf29b-154">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cf29b-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="cf29b-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="cf29b-155">lastRefreshDateTime</span></span>|<span data-ttu-id="cf29b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf29b-156">DateTimeOffset</span></span>|<span data-ttu-id="cf29b-157">Время последнего обновления кэшного отчета</span><span class="sxs-lookup"><span data-stu-id="cf29b-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="cf29b-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cf29b-158">expirationDateTime</span></span>|<span data-ttu-id="cf29b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf29b-159">DateTimeOffset</span></span>|<span data-ttu-id="cf29b-160">Время истечения срока действия кэш-отчета</span><span class="sxs-lookup"><span data-stu-id="cf29b-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="cf29b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf29b-161">Response</span></span>
<span data-ttu-id="cf29b-162">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf29b-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf29b-163">Пример</span><span class="sxs-lookup"><span data-stu-id="cf29b-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf29b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf29b-164">Request</span></span>
<span data-ttu-id="cf29b-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf29b-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="cf29b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf29b-166">Response</span></span>
<span data-ttu-id="cf29b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf29b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "46947722-7722-4694-2277-944622779446",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




