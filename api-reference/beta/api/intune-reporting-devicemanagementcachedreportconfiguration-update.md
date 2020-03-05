---
title: Обновление Девицеманажементкачедрепортконфигуратион
description: Обновление свойств объекта Девицеманажементкачедрепортконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94e0c6128ea3da59ffabf366581f74d2f78d75b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459241"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="58a70-103">Обновление Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="58a70-103">Update deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="58a70-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="58a70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58a70-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58a70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a70-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58a70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a70-107">Обновление свойств объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58a70-107">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a70-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58a70-108">Prerequisites</span></span>
<span data-ttu-id="58a70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58a70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58a70-111">Permission type</span></span>|<span data-ttu-id="58a70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58a70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58a70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58a70-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="58a70-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58a70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58a70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58a70-116">Not supported.</span></span>|
|<span data-ttu-id="58a70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58a70-117">Application</span></span>|<span data-ttu-id="58a70-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="58a70-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58a70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58a70-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58a70-120">Request headers</span></span>
|<span data-ttu-id="58a70-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58a70-121">Header</span></span>|<span data-ttu-id="58a70-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58a70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a70-123">Authorization</span></span>|<span data-ttu-id="58a70-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58a70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a70-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58a70-125">Accept</span></span>|<span data-ttu-id="58a70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58a70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a70-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58a70-127">Request body</span></span>
<span data-ttu-id="58a70-128">В тексте запроса добавьте представление объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58a70-128">In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

<span data-ttu-id="58a70-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a70-129">The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>

|<span data-ttu-id="58a70-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="58a70-130">Property</span></span>|<span data-ttu-id="58a70-131">Тип</span><span class="sxs-lookup"><span data-stu-id="58a70-131">Type</span></span>|<span data-ttu-id="58a70-132">Описание</span><span class="sxs-lookup"><span data-stu-id="58a70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a70-133">id</span><span class="sxs-lookup"><span data-stu-id="58a70-133">id</span></span>|<span data-ttu-id="58a70-134">String</span><span class="sxs-lookup"><span data-stu-id="58a70-134">String</span></span>|<span data-ttu-id="58a70-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="58a70-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="58a70-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="58a70-136">reportName</span></span>|<span data-ttu-id="58a70-137">String</span><span class="sxs-lookup"><span data-stu-id="58a70-137">String</span></span>|<span data-ttu-id="58a70-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="58a70-138">Name of the report</span></span>|
|<span data-ttu-id="58a70-139">filter</span><span class="sxs-lookup"><span data-stu-id="58a70-139">filter</span></span>|<span data-ttu-id="58a70-140">String</span><span class="sxs-lookup"><span data-stu-id="58a70-140">String</span></span>|<span data-ttu-id="58a70-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="58a70-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="58a70-142">select</span><span class="sxs-lookup"><span data-stu-id="58a70-142">select</span></span>|<span data-ttu-id="58a70-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="58a70-143">String collection</span></span>|<span data-ttu-id="58a70-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="58a70-144">Columns selected from the report</span></span>|
|<span data-ttu-id="58a70-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="58a70-145">orderBy</span></span>|<span data-ttu-id="58a70-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="58a70-146">String collection</span></span>|<span data-ttu-id="58a70-147">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="58a70-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="58a70-148">status</span><span class="sxs-lookup"><span data-stu-id="58a70-148">status</span></span>|[<span data-ttu-id="58a70-149">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="58a70-149">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="58a70-150">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="58a70-150">Status of the cached report.</span></span> <span data-ttu-id="58a70-151">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="58a70-151">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="58a70-152">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="58a70-152">lastRefreshDateTime</span></span>|<span data-ttu-id="58a70-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a70-153">DateTimeOffset</span></span>|<span data-ttu-id="58a70-154">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="58a70-154">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="58a70-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58a70-155">expirationDateTime</span></span>|<span data-ttu-id="58a70-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a70-156">DateTimeOffset</span></span>|<span data-ttu-id="58a70-157">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="58a70-157">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="58a70-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a70-158">Response</span></span>
<span data-ttu-id="58a70-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58a70-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a70-160">Пример</span><span class="sxs-lookup"><span data-stu-id="58a70-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a70-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a70-161">Request</span></span>
<span data-ttu-id="58a70-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58a70-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58a70-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a70-163">Response</span></span>
<span data-ttu-id="58a70-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58a70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





