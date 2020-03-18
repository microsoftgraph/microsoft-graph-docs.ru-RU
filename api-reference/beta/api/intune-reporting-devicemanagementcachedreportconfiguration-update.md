---
title: Обновление Девицеманажементкачедрепортконфигуратион
description: Обновление свойств объекта Девицеманажементкачедрепортконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f4ea7ad8e14331cd7d9b322cf977f59ff452efc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801448"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="98dd3-103">Обновление Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="98dd3-103">Update deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="98dd3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98dd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98dd3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98dd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98dd3-106">Обновление свойств объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="98dd3-106">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98dd3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98dd3-107">Prerequisites</span></span>
<span data-ttu-id="98dd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98dd3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98dd3-110">Permission type</span></span>|<span data-ttu-id="98dd3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98dd3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98dd3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98dd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98dd3-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="98dd3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="98dd3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98dd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98dd3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98dd3-115">Not supported.</span></span>|
|<span data-ttu-id="98dd3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="98dd3-116">Application</span></span>|<span data-ttu-id="98dd3-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="98dd3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98dd3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98dd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="98dd3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98dd3-119">Request headers</span></span>
|<span data-ttu-id="98dd3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98dd3-120">Header</span></span>|<span data-ttu-id="98dd3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98dd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98dd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98dd3-122">Authorization</span></span>|<span data-ttu-id="98dd3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98dd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98dd3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98dd3-124">Accept</span></span>|<span data-ttu-id="98dd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98dd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98dd3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98dd3-126">Request body</span></span>
<span data-ttu-id="98dd3-127">В тексте запроса добавьте представление объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98dd3-127">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="98dd3-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98dd3-128">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="98dd3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="98dd3-129">Property</span></span>|<span data-ttu-id="98dd3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="98dd3-130">Type</span></span>|<span data-ttu-id="98dd3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="98dd3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98dd3-132">id</span><span class="sxs-lookup"><span data-stu-id="98dd3-132">id</span></span>|<span data-ttu-id="98dd3-133">String</span><span class="sxs-lookup"><span data-stu-id="98dd3-133">String</span></span>|<span data-ttu-id="98dd3-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="98dd3-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="98dd3-135">репортнаме</span><span class="sxs-lookup"><span data-stu-id="98dd3-135">reportName</span></span>|<span data-ttu-id="98dd3-136">String</span><span class="sxs-lookup"><span data-stu-id="98dd3-136">String</span></span>|<span data-ttu-id="98dd3-137">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="98dd3-137">Name of the report</span></span>|
|<span data-ttu-id="98dd3-138">filter</span><span class="sxs-lookup"><span data-stu-id="98dd3-138">filter</span></span>|<span data-ttu-id="98dd3-139">String</span><span class="sxs-lookup"><span data-stu-id="98dd3-139">String</span></span>|<span data-ttu-id="98dd3-140">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="98dd3-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="98dd3-141">select</span><span class="sxs-lookup"><span data-stu-id="98dd3-141">select</span></span>|<span data-ttu-id="98dd3-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="98dd3-142">String collection</span></span>|<span data-ttu-id="98dd3-143">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="98dd3-143">Columns selected from the report</span></span>|
|<span data-ttu-id="98dd3-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="98dd3-144">orderBy</span></span>|<span data-ttu-id="98dd3-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="98dd3-145">String collection</span></span>|<span data-ttu-id="98dd3-146">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="98dd3-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="98dd3-147">status</span><span class="sxs-lookup"><span data-stu-id="98dd3-147">status</span></span>|[<span data-ttu-id="98dd3-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="98dd3-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="98dd3-149">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="98dd3-149">Status of the cached report.</span></span> <span data-ttu-id="98dd3-150">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="98dd3-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="98dd3-151">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="98dd3-151">lastRefreshDateTime</span></span>|<span data-ttu-id="98dd3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98dd3-152">DateTimeOffset</span></span>|<span data-ttu-id="98dd3-153">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="98dd3-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="98dd3-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="98dd3-154">expirationDateTime</span></span>|<span data-ttu-id="98dd3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98dd3-155">DateTimeOffset</span></span>|<span data-ttu-id="98dd3-156">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="98dd3-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="98dd3-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="98dd3-157">Response</span></span>
<span data-ttu-id="98dd3-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98dd3-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98dd3-159">Пример</span><span class="sxs-lookup"><span data-stu-id="98dd3-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="98dd3-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="98dd3-160">Request</span></span>
<span data-ttu-id="98dd3-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98dd3-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
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

### <a name="response"></a><span data-ttu-id="98dd3-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="98dd3-162">Response</span></span>
<span data-ttu-id="98dd3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98dd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




