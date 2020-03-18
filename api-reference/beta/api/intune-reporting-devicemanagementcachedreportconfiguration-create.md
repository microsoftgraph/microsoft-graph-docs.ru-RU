---
title: Создание Девицеманажементкачедрепортконфигуратион
description: Создание нового объекта Девицеманажементкачедрепортконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f0447c2ec79d7755ac09c35984c4d68ecc4c275
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801476"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="82d92-103">Создание Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="82d92-103">Create deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="82d92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82d92-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82d92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d92-106">Создание нового объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82d92-106">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82d92-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82d92-107">Prerequisites</span></span>
<span data-ttu-id="82d92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82d92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d92-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82d92-110">Permission type</span></span>|<span data-ttu-id="82d92-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82d92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82d92-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82d92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82d92-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="82d92-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="82d92-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82d92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82d92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d92-115">Not supported.</span></span>|
|<span data-ttu-id="82d92-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="82d92-116">Application</span></span>|<span data-ttu-id="82d92-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="82d92-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82d92-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82d92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82d92-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82d92-119">Request headers</span></span>
|<span data-ttu-id="82d92-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82d92-120">Header</span></span>|<span data-ttu-id="82d92-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82d92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82d92-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d92-122">Authorization</span></span>|<span data-ttu-id="82d92-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82d92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82d92-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82d92-124">Accept</span></span>|<span data-ttu-id="82d92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82d92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82d92-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82d92-126">Request body</span></span>
<span data-ttu-id="82d92-127">В тексте запроса добавьте представление объекта Девицеманажементкачедрепортконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82d92-127">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="82d92-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкачедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="82d92-128">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="82d92-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82d92-129">Property</span></span>|<span data-ttu-id="82d92-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82d92-130">Type</span></span>|<span data-ttu-id="82d92-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82d92-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d92-132">id</span><span class="sxs-lookup"><span data-stu-id="82d92-132">id</span></span>|<span data-ttu-id="82d92-133">String</span><span class="sxs-lookup"><span data-stu-id="82d92-133">String</span></span>|<span data-ttu-id="82d92-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="82d92-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="82d92-135">репортнаме</span><span class="sxs-lookup"><span data-stu-id="82d92-135">reportName</span></span>|<span data-ttu-id="82d92-136">String</span><span class="sxs-lookup"><span data-stu-id="82d92-136">String</span></span>|<span data-ttu-id="82d92-137">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="82d92-137">Name of the report</span></span>|
|<span data-ttu-id="82d92-138">filter</span><span class="sxs-lookup"><span data-stu-id="82d92-138">filter</span></span>|<span data-ttu-id="82d92-139">String</span><span class="sxs-lookup"><span data-stu-id="82d92-139">String</span></span>|<span data-ttu-id="82d92-140">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="82d92-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="82d92-141">select</span><span class="sxs-lookup"><span data-stu-id="82d92-141">select</span></span>|<span data-ttu-id="82d92-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82d92-142">String collection</span></span>|<span data-ttu-id="82d92-143">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="82d92-143">Columns selected from the report</span></span>|
|<span data-ttu-id="82d92-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="82d92-144">orderBy</span></span>|<span data-ttu-id="82d92-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82d92-145">String collection</span></span>|<span data-ttu-id="82d92-146">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="82d92-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="82d92-147">status</span><span class="sxs-lookup"><span data-stu-id="82d92-147">status</span></span>|[<span data-ttu-id="82d92-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="82d92-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="82d92-149">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="82d92-149">Status of the cached report.</span></span> <span data-ttu-id="82d92-150">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="82d92-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="82d92-151">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="82d92-151">lastRefreshDateTime</span></span>|<span data-ttu-id="82d92-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82d92-152">DateTimeOffset</span></span>|<span data-ttu-id="82d92-153">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="82d92-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="82d92-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="82d92-154">expirationDateTime</span></span>|<span data-ttu-id="82d92-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82d92-155">DateTimeOffset</span></span>|<span data-ttu-id="82d92-156">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="82d92-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="82d92-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d92-157">Response</span></span>
<span data-ttu-id="82d92-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82d92-158">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82d92-159">Пример</span><span class="sxs-lookup"><span data-stu-id="82d92-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="82d92-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="82d92-160">Request</span></span>
<span data-ttu-id="82d92-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82d92-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
Content-type: application/json
Content-length: 385

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
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a><span data-ttu-id="82d92-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d92-162">Response</span></span>
<span data-ttu-id="82d92-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82d92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

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
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




