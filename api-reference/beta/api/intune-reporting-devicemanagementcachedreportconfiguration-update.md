---
title: Обновление Девицеманажементкачедрепортконфигуратион
description: Обновление свойств объекта Девицеманажементкачедрепортконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f43a7b91931ba777909df75facb91d488033ca9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791344"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="99af6-103">Обновление Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="99af6-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="99af6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99af6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99af6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99af6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99af6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99af6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99af6-107">Обновление свойств объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="99af6-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99af6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99af6-108">Prerequisites</span></span>
<span data-ttu-id="99af6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99af6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99af6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99af6-111">Permission type</span></span>|<span data-ttu-id="99af6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99af6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99af6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99af6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99af6-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="99af6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99af6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99af6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99af6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99af6-116">Not supported.</span></span>|
|<span data-ttu-id="99af6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99af6-117">Application</span></span>|<span data-ttu-id="99af6-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="99af6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99af6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99af6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="99af6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99af6-120">Request headers</span></span>
|<span data-ttu-id="99af6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99af6-121">Header</span></span>|<span data-ttu-id="99af6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99af6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99af6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99af6-123">Authorization</span></span>|<span data-ttu-id="99af6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99af6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99af6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99af6-125">Accept</span></span>|<span data-ttu-id="99af6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99af6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99af6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99af6-127">Request body</span></span>
<span data-ttu-id="99af6-128">В тексте запроса добавьте представление объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99af6-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="99af6-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99af6-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="99af6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99af6-130">Property</span></span>|<span data-ttu-id="99af6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99af6-131">Type</span></span>|<span data-ttu-id="99af6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99af6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99af6-133">id</span><span class="sxs-lookup"><span data-stu-id="99af6-133">id</span></span>|<span data-ttu-id="99af6-134">String</span><span class="sxs-lookup"><span data-stu-id="99af6-134">String</span></span>|<span data-ttu-id="99af6-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="99af6-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="99af6-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="99af6-136">reportName</span></span>|<span data-ttu-id="99af6-137">String</span><span class="sxs-lookup"><span data-stu-id="99af6-137">String</span></span>|<span data-ttu-id="99af6-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="99af6-138">Name of the report</span></span>|
|<span data-ttu-id="99af6-139">filter</span><span class="sxs-lookup"><span data-stu-id="99af6-139">filter</span></span>|<span data-ttu-id="99af6-140">String</span><span class="sxs-lookup"><span data-stu-id="99af6-140">String</span></span>|<span data-ttu-id="99af6-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="99af6-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="99af6-142">select</span><span class="sxs-lookup"><span data-stu-id="99af6-142">select</span></span>|<span data-ttu-id="99af6-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99af6-143">String collection</span></span>|<span data-ttu-id="99af6-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="99af6-144">Columns selected from the report</span></span>|
|<span data-ttu-id="99af6-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="99af6-145">orderBy</span></span>|<span data-ttu-id="99af6-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99af6-146">String collection</span></span>|<span data-ttu-id="99af6-147">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="99af6-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="99af6-148">метаданных</span><span class="sxs-lookup"><span data-stu-id="99af6-148">metadata</span></span>|<span data-ttu-id="99af6-149">String</span><span class="sxs-lookup"><span data-stu-id="99af6-149">String</span></span>|<span data-ttu-id="99af6-150">Управляемые вызывающими метаданными метаданные, связанные с отчетом</span><span class="sxs-lookup"><span data-stu-id="99af6-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="99af6-151">status</span><span class="sxs-lookup"><span data-stu-id="99af6-151">status</span></span>|[<span data-ttu-id="99af6-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="99af6-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="99af6-153">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="99af6-153">Status of the cached report.</span></span> <span data-ttu-id="99af6-154">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="99af6-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="99af6-155">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="99af6-155">lastRefreshDateTime</span></span>|<span data-ttu-id="99af6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99af6-156">DateTimeOffset</span></span>|<span data-ttu-id="99af6-157">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="99af6-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="99af6-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="99af6-158">expirationDateTime</span></span>|<span data-ttu-id="99af6-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99af6-159">DateTimeOffset</span></span>|<span data-ttu-id="99af6-160">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="99af6-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="99af6-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="99af6-161">Response</span></span>
<span data-ttu-id="99af6-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99af6-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99af6-163">Пример</span><span class="sxs-lookup"><span data-stu-id="99af6-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="99af6-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="99af6-164">Request</span></span>
<span data-ttu-id="99af6-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99af6-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99af6-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="99af6-166">Response</span></span>
<span data-ttu-id="99af6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99af6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



