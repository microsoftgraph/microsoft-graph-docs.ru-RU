---
title: Создание Девицеманажементкачедрепортконфигуратион
description: Создание нового объекта Девицеманажементкачедрепортконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d58fb51a8577575643d33c3b97c107cd3130f77f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698325"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="7e26d-103">Создание Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7e26d-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="7e26d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e26d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e26d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e26d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e26d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e26d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e26d-107">Создание нового объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7e26d-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e26d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e26d-108">Prerequisites</span></span>
<span data-ttu-id="7e26d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e26d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e26d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e26d-111">Permission type</span></span>|<span data-ttu-id="7e26d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e26d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e26d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e26d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e26d-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e26d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7e26d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e26d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e26d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e26d-116">Not supported.</span></span>|
|<span data-ttu-id="7e26d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e26d-117">Application</span></span>|<span data-ttu-id="7e26d-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e26d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e26d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e26d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e26d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e26d-120">Request headers</span></span>
|<span data-ttu-id="7e26d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e26d-121">Header</span></span>|<span data-ttu-id="7e26d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7e26d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e26d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e26d-123">Authorization</span></span>|<span data-ttu-id="7e26d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e26d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e26d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e26d-125">Accept</span></span>|<span data-ttu-id="7e26d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e26d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e26d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e26d-127">Request body</span></span>
<span data-ttu-id="7e26d-128">В тексте запроса добавьте представление объекта Девицеманажементкачедрепортконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e26d-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="7e26d-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкачедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="7e26d-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="7e26d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e26d-130">Property</span></span>|<span data-ttu-id="7e26d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7e26d-131">Type</span></span>|<span data-ttu-id="7e26d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7e26d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e26d-133">id</span><span class="sxs-lookup"><span data-stu-id="7e26d-133">id</span></span>|<span data-ttu-id="7e26d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7e26d-134">String</span></span>|<span data-ttu-id="7e26d-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="7e26d-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="7e26d-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="7e26d-136">reportName</span></span>|<span data-ttu-id="7e26d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7e26d-137">String</span></span>|<span data-ttu-id="7e26d-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="7e26d-138">Name of the report</span></span>|
|<span data-ttu-id="7e26d-139">filter</span><span class="sxs-lookup"><span data-stu-id="7e26d-139">filter</span></span>|<span data-ttu-id="7e26d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7e26d-140">String</span></span>|<span data-ttu-id="7e26d-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="7e26d-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="7e26d-142">select</span><span class="sxs-lookup"><span data-stu-id="7e26d-142">select</span></span>|<span data-ttu-id="7e26d-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7e26d-143">String collection</span></span>|<span data-ttu-id="7e26d-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="7e26d-144">Columns selected from the report</span></span>|
|<span data-ttu-id="7e26d-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="7e26d-145">orderBy</span></span>|<span data-ttu-id="7e26d-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7e26d-146">String collection</span></span>|<span data-ttu-id="7e26d-147">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="7e26d-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="7e26d-148">метаданных</span><span class="sxs-lookup"><span data-stu-id="7e26d-148">metadata</span></span>|<span data-ttu-id="7e26d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="7e26d-149">String</span></span>|<span data-ttu-id="7e26d-150">Управляемые вызывающими метаданными метаданные, связанные с отчетом</span><span class="sxs-lookup"><span data-stu-id="7e26d-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="7e26d-151">status</span><span class="sxs-lookup"><span data-stu-id="7e26d-151">status</span></span>|[<span data-ttu-id="7e26d-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="7e26d-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="7e26d-153">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="7e26d-153">Status of the cached report.</span></span> <span data-ttu-id="7e26d-154">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7e26d-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="7e26d-155">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="7e26d-155">lastRefreshDateTime</span></span>|<span data-ttu-id="7e26d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e26d-156">DateTimeOffset</span></span>|<span data-ttu-id="7e26d-157">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="7e26d-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="7e26d-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e26d-158">expirationDateTime</span></span>|<span data-ttu-id="7e26d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e26d-159">DateTimeOffset</span></span>|<span data-ttu-id="7e26d-160">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="7e26d-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="7e26d-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e26d-161">Response</span></span>
<span data-ttu-id="7e26d-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e26d-162">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e26d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="7e26d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e26d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e26d-164">Request</span></span>
<span data-ttu-id="7e26d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e26d-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e26d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e26d-166">Response</span></span>
<span data-ttu-id="7e26d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e26d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





