---
title: Создание Девицеманажементкачедрепортконфигуратион
description: Создание нового объекта Девицеманажементкачедрепортконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10c326a7862bcd0670ec55976f459736665c6afa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459304"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="a6c2d-103">Создание Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a6c2d-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="a6c2d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a6c2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6c2d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6c2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6c2d-107">Создание нового объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c2d-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6c2d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6c2d-108">Prerequisites</span></span>
<span data-ttu-id="a6c2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c2d-111">Permission type</span></span>|<span data-ttu-id="a6c2d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6c2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6c2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c2d-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a6c2d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c2d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6c2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-116">Not supported.</span></span>|
|<span data-ttu-id="a6c2d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6c2d-117">Application</span></span>|<span data-ttu-id="a6c2d-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a6c2d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c2d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6c2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6c2d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a6c2d-120">Request headers</span></span>
|<span data-ttu-id="a6c2d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6c2d-121">Header</span></span>|<span data-ttu-id="a6c2d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a6c2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c2d-123">Authorization</span></span>|<span data-ttu-id="a6c2d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c2d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6c2d-125">Accept</span></span>|<span data-ttu-id="a6c2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c2d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6c2d-127">Request body</span></span>
<span data-ttu-id="a6c2d-128">В тексте запроса добавьте представление объекта Девицеманажементкачедрепортконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="a6c2d-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкачедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="a6c2d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6c2d-130">Property</span></span>|<span data-ttu-id="a6c2d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c2d-131">Type</span></span>|<span data-ttu-id="a6c2d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c2d-133">id</span><span class="sxs-lookup"><span data-stu-id="a6c2d-133">id</span></span>|<span data-ttu-id="a6c2d-134">String</span><span class="sxs-lookup"><span data-stu-id="a6c2d-134">String</span></span>|<span data-ttu-id="a6c2d-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="a6c2d-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="a6c2d-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="a6c2d-136">reportName</span></span>|<span data-ttu-id="a6c2d-137">String</span><span class="sxs-lookup"><span data-stu-id="a6c2d-137">String</span></span>|<span data-ttu-id="a6c2d-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="a6c2d-138">Name of the report</span></span>|
|<span data-ttu-id="a6c2d-139">filter</span><span class="sxs-lookup"><span data-stu-id="a6c2d-139">filter</span></span>|<span data-ttu-id="a6c2d-140">String</span><span class="sxs-lookup"><span data-stu-id="a6c2d-140">String</span></span>|<span data-ttu-id="a6c2d-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="a6c2d-142">select</span><span class="sxs-lookup"><span data-stu-id="a6c2d-142">select</span></span>|<span data-ttu-id="a6c2d-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a6c2d-143">String collection</span></span>|<span data-ttu-id="a6c2d-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="a6c2d-144">Columns selected from the report</span></span>|
|<span data-ttu-id="a6c2d-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="a6c2d-145">orderBy</span></span>|<span data-ttu-id="a6c2d-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a6c2d-146">String collection</span></span>|<span data-ttu-id="a6c2d-147">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="a6c2d-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="a6c2d-148">status</span><span class="sxs-lookup"><span data-stu-id="a6c2d-148">status</span></span>|[<span data-ttu-id="a6c2d-149">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="a6c2d-149">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="a6c2d-150">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-150">Status of the cached report.</span></span> <span data-ttu-id="a6c2d-151">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-151">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a6c2d-152">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="a6c2d-152">lastRefreshDateTime</span></span>|<span data-ttu-id="a6c2d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c2d-153">DateTimeOffset</span></span>|<span data-ttu-id="a6c2d-154">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="a6c2d-154">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="a6c2d-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c2d-155">expirationDateTime</span></span>|<span data-ttu-id="a6c2d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c2d-156">DateTimeOffset</span></span>|<span data-ttu-id="a6c2d-157">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="a6c2d-157">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="a6c2d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c2d-158">Response</span></span>
<span data-ttu-id="a6c2d-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-159">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c2d-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a6c2d-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6c2d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6c2d-161">Request</span></span>
<span data-ttu-id="a6c2d-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6c2d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c2d-163">Response</span></span>
<span data-ttu-id="a6c2d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6c2d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





