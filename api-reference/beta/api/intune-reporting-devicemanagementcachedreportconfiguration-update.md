---
title: Обновление Девицеманажементкачедрепортконфигуратион
description: Обновление свойств объекта Девицеманажементкачедрепортконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2308fc686358f28c3ffb3c7aff523207a7e46d8b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537291"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="de679-103">Обновление Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="de679-103">Update deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="de679-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de679-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de679-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de679-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de679-106">Обновление свойств объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="de679-106">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de679-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de679-107">Prerequisites</span></span>
<span data-ttu-id="de679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de679-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de679-110">Permission type</span></span>|<span data-ttu-id="de679-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de679-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de679-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de679-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de679-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de679-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="de679-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de679-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de679-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de679-115">Not supported.</span></span>|
|<span data-ttu-id="de679-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="de679-116">Application</span></span>|<span data-ttu-id="de679-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de679-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de679-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de679-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="de679-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de679-119">Request headers</span></span>
|<span data-ttu-id="de679-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de679-120">Header</span></span>|<span data-ttu-id="de679-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de679-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de679-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de679-122">Authorization</span></span>|<span data-ttu-id="de679-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de679-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de679-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de679-124">Accept</span></span>|<span data-ttu-id="de679-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de679-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de679-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de679-126">Request body</span></span>
<span data-ttu-id="de679-127">В тексте запроса добавьте представление объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de679-127">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="de679-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de679-128">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="de679-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="de679-129">Property</span></span>|<span data-ttu-id="de679-130">Тип</span><span class="sxs-lookup"><span data-stu-id="de679-130">Type</span></span>|<span data-ttu-id="de679-131">Описание</span><span class="sxs-lookup"><span data-stu-id="de679-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de679-132">id</span><span class="sxs-lookup"><span data-stu-id="de679-132">id</span></span>|<span data-ttu-id="de679-133">String</span><span class="sxs-lookup"><span data-stu-id="de679-133">String</span></span>|<span data-ttu-id="de679-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="de679-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="de679-135">репортнаме</span><span class="sxs-lookup"><span data-stu-id="de679-135">reportName</span></span>|<span data-ttu-id="de679-136">String</span><span class="sxs-lookup"><span data-stu-id="de679-136">String</span></span>|<span data-ttu-id="de679-137">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="de679-137">Name of the report</span></span>|
|<span data-ttu-id="de679-138">filter</span><span class="sxs-lookup"><span data-stu-id="de679-138">filter</span></span>|<span data-ttu-id="de679-139">String</span><span class="sxs-lookup"><span data-stu-id="de679-139">String</span></span>|<span data-ttu-id="de679-140">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="de679-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="de679-141">select</span><span class="sxs-lookup"><span data-stu-id="de679-141">select</span></span>|<span data-ttu-id="de679-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de679-142">String collection</span></span>|<span data-ttu-id="de679-143">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="de679-143">Columns selected from the report</span></span>|
|<span data-ttu-id="de679-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="de679-144">orderBy</span></span>|<span data-ttu-id="de679-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de679-145">String collection</span></span>|<span data-ttu-id="de679-146">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="de679-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="de679-147">status</span><span class="sxs-lookup"><span data-stu-id="de679-147">status</span></span>|[<span data-ttu-id="de679-148">девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="de679-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="de679-149">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="de679-149">Status of the cached report.</span></span> <span data-ttu-id="de679-150">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="de679-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="de679-151">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="de679-151">lastRefreshDateTime</span></span>|<span data-ttu-id="de679-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de679-152">DateTimeOffset</span></span>|<span data-ttu-id="de679-153">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="de679-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="de679-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="de679-154">expirationDateTime</span></span>|<span data-ttu-id="de679-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de679-155">DateTimeOffset</span></span>|<span data-ttu-id="de679-156">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="de679-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="de679-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="de679-157">Response</span></span>
<span data-ttu-id="de679-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de679-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de679-159">Пример</span><span class="sxs-lookup"><span data-stu-id="de679-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="de679-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="de679-160">Request</span></span>
<span data-ttu-id="de679-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de679-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de679-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="de679-162">Response</span></span>
<span data-ttu-id="de679-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de679-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






