---
title: Создание deviceManagementCachedReportConfiguration
description: Создание нового объекта deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9df14360ac503b20eaf881fb37a79c111c8c2c2a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51124605"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="3d526-103">Создание deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d526-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="3d526-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d526-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d526-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d526-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d526-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d526-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d526-107">Создание нового [объекта deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d526-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d526-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d526-108">Prerequisites</span></span>
<span data-ttu-id="3d526-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d526-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d526-111">Permission type</span></span>|<span data-ttu-id="3d526-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d526-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d526-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d526-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d526-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d526-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d526-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d526-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d526-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d526-116">Not supported.</span></span>|
|<span data-ttu-id="3d526-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3d526-117">Application</span></span>|<span data-ttu-id="3d526-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d526-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d526-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d526-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d526-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d526-120">Request headers</span></span>
|<span data-ttu-id="3d526-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d526-121">Header</span></span>|<span data-ttu-id="3d526-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d526-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d526-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d526-123">Authorization</span></span>|<span data-ttu-id="3d526-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d526-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d526-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d526-125">Accept</span></span>|<span data-ttu-id="3d526-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d526-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d526-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d526-127">Request body</span></span>
<span data-ttu-id="3d526-128">В теле запроса поставляем представление JSON для объекта deviceManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d526-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="3d526-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementCachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d526-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="3d526-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d526-130">Property</span></span>|<span data-ttu-id="3d526-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d526-131">Type</span></span>|<span data-ttu-id="3d526-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d526-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d526-133">id</span><span class="sxs-lookup"><span data-stu-id="3d526-133">id</span></span>|<span data-ttu-id="3d526-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3d526-134">String</span></span>|<span data-ttu-id="3d526-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="3d526-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="3d526-136">reportName</span><span class="sxs-lookup"><span data-stu-id="3d526-136">reportName</span></span>|<span data-ttu-id="3d526-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3d526-137">String</span></span>|<span data-ttu-id="3d526-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="3d526-138">Name of the report</span></span>|
|<span data-ttu-id="3d526-139">filter</span><span class="sxs-lookup"><span data-stu-id="3d526-139">filter</span></span>|<span data-ttu-id="3d526-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3d526-140">String</span></span>|<span data-ttu-id="3d526-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="3d526-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="3d526-142">select</span><span class="sxs-lookup"><span data-stu-id="3d526-142">select</span></span>|<span data-ttu-id="3d526-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3d526-143">String collection</span></span>|<span data-ttu-id="3d526-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="3d526-144">Columns selected from the report</span></span>|
|<span data-ttu-id="3d526-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="3d526-145">orderBy</span></span>|<span data-ttu-id="3d526-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3d526-146">String collection</span></span>|<span data-ttu-id="3d526-147">Порядок столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="3d526-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="3d526-148">метаданные</span><span class="sxs-lookup"><span data-stu-id="3d526-148">metadata</span></span>|<span data-ttu-id="3d526-149">Строка</span><span class="sxs-lookup"><span data-stu-id="3d526-149">String</span></span>|<span data-ttu-id="3d526-150">Метаданные, управляемые вызывателями, связанные с отчетом</span><span class="sxs-lookup"><span data-stu-id="3d526-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="3d526-151">status</span><span class="sxs-lookup"><span data-stu-id="3d526-151">status</span></span>|[<span data-ttu-id="3d526-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="3d526-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="3d526-153">Состояние кэшного отчета.</span><span class="sxs-lookup"><span data-stu-id="3d526-153">Status of the cached report.</span></span> <span data-ttu-id="3d526-154">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3d526-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="3d526-155">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="3d526-155">lastRefreshDateTime</span></span>|<span data-ttu-id="3d526-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d526-156">DateTimeOffset</span></span>|<span data-ttu-id="3d526-157">Время последнего обновления кэшного отчета</span><span class="sxs-lookup"><span data-stu-id="3d526-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="3d526-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d526-158">expirationDateTime</span></span>|<span data-ttu-id="3d526-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d526-159">DateTimeOffset</span></span>|<span data-ttu-id="3d526-160">Время истечения срока действия кэш-отчета</span><span class="sxs-lookup"><span data-stu-id="3d526-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="3d526-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d526-161">Response</span></span>
<span data-ttu-id="3d526-162">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3d526-162">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d526-163">Пример</span><span class="sxs-lookup"><span data-stu-id="3d526-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d526-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d526-164">Request</span></span>
<span data-ttu-id="3d526-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d526-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
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

### <a name="response"></a><span data-ttu-id="3d526-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d526-166">Response</span></span>
<span data-ttu-id="3d526-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d526-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




