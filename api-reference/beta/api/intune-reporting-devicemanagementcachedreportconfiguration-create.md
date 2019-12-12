---
title: Создание Девицеманажементкачедрепортконфигуратион
description: Создание нового объекта Девицеманажементкачедрепортконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 240ca89d363f60eff21cc1d299b5b96c5523cbbc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955079"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="a5c3e-103">Создание Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a5c3e-103">Create deviceManagementCachedReportConfiguration</span></span>

> <span data-ttu-id="a5c3e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5c3e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5c3e-106">Создание нового объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a5c3e-106">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5c3e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a5c3e-107">Prerequisites</span></span>
<span data-ttu-id="a5c3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c3e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c3e-110">Permission type</span></span>|<span data-ttu-id="a5c3e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5c3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5c3e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5c3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5c3e-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a5c3e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a5c3e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5c3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5c3e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-115">Not supported.</span></span>|
|<span data-ttu-id="a5c3e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5c3e-116">Application</span></span>|<span data-ttu-id="a5c3e-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a5c3e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5c3e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5c3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a5c3e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5c3e-119">Request headers</span></span>
|<span data-ttu-id="a5c3e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5c3e-120">Header</span></span>|<span data-ttu-id="a5c3e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a5c3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5c3e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5c3e-122">Authorization</span></span>|<span data-ttu-id="a5c3e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5c3e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5c3e-124">Accept</span></span>|<span data-ttu-id="a5c3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5c3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5c3e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5c3e-126">Request body</span></span>
<span data-ttu-id="a5c3e-127">В тексте запроса добавьте представление объекта Девицеманажементкачедрепортконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-127">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="a5c3e-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкачедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-128">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="a5c3e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5c3e-129">Property</span></span>|<span data-ttu-id="a5c3e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5c3e-130">Type</span></span>|<span data-ttu-id="a5c3e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c3e-132">id</span><span class="sxs-lookup"><span data-stu-id="a5c3e-132">id</span></span>|<span data-ttu-id="a5c3e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a5c3e-133">String</span></span>|<span data-ttu-id="a5c3e-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="a5c3e-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="a5c3e-135">репортнаме</span><span class="sxs-lookup"><span data-stu-id="a5c3e-135">reportName</span></span>|<span data-ttu-id="a5c3e-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a5c3e-136">String</span></span>|<span data-ttu-id="a5c3e-137">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="a5c3e-137">Name of the report</span></span>|
|<span data-ttu-id="a5c3e-138">filter</span><span class="sxs-lookup"><span data-stu-id="a5c3e-138">filter</span></span>|<span data-ttu-id="a5c3e-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a5c3e-139">String</span></span>|<span data-ttu-id="a5c3e-140">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-140">Filters applied on report creation.</span></span>|
|<span data-ttu-id="a5c3e-141">select</span><span class="sxs-lookup"><span data-stu-id="a5c3e-141">select</span></span>|<span data-ttu-id="a5c3e-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a5c3e-142">String collection</span></span>|<span data-ttu-id="a5c3e-143">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="a5c3e-143">Columns selected from the report</span></span>|
|<span data-ttu-id="a5c3e-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="a5c3e-144">orderBy</span></span>|<span data-ttu-id="a5c3e-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a5c3e-145">String collection</span></span>|<span data-ttu-id="a5c3e-146">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="a5c3e-146">Ordering of columns in the report</span></span>|
|<span data-ttu-id="a5c3e-147">status</span><span class="sxs-lookup"><span data-stu-id="a5c3e-147">status</span></span>|[<span data-ttu-id="a5c3e-148">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="a5c3e-148">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="a5c3e-149">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-149">Status of the cached report.</span></span> <span data-ttu-id="a5c3e-150">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-150">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a5c3e-151">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="a5c3e-151">lastRefreshDateTime</span></span>|<span data-ttu-id="a5c3e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c3e-152">DateTimeOffset</span></span>|<span data-ttu-id="a5c3e-153">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="a5c3e-153">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="a5c3e-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c3e-154">expirationDateTime</span></span>|<span data-ttu-id="a5c3e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c3e-155">DateTimeOffset</span></span>|<span data-ttu-id="a5c3e-156">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="a5c3e-156">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="a5c3e-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5c3e-157">Response</span></span>
<span data-ttu-id="a5c3e-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-158">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5c3e-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a5c3e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5c3e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c3e-160">Request</span></span>
<span data-ttu-id="a5c3e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5c3e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c3e-162">Response</span></span>
<span data-ttu-id="a5c3e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5c3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





