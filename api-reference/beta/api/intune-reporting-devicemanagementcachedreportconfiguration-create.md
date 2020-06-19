---
title: Создание Девицеманажементкачедрепортконфигуратион
description: Создание нового объекта Девицеманажементкачедрепортконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7340fffa01f99c33433c60b08b12748a2505cfae
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791365"
---
# <a name="create-devicemanagementcachedreportconfiguration"></a><span data-ttu-id="9223c-103">Создание Девицеманажементкачедрепортконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9223c-103">Create deviceManagementCachedReportConfiguration</span></span>

<span data-ttu-id="9223c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9223c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9223c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9223c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9223c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9223c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9223c-107">Создание нового объекта [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9223c-107">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9223c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9223c-108">Prerequisites</span></span>
<span data-ttu-id="9223c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9223c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9223c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9223c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9223c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9223c-111">Permission type</span></span>|<span data-ttu-id="9223c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9223c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9223c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9223c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9223c-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9223c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9223c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9223c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9223c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9223c-116">Not supported.</span></span>|
|<span data-ttu-id="9223c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9223c-117">Application</span></span>|<span data-ttu-id="9223c-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9223c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9223c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9223c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9223c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9223c-120">Request headers</span></span>
|<span data-ttu-id="9223c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9223c-121">Header</span></span>|<span data-ttu-id="9223c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9223c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9223c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9223c-123">Authorization</span></span>|<span data-ttu-id="9223c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9223c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9223c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9223c-125">Accept</span></span>|<span data-ttu-id="9223c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9223c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9223c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9223c-127">Request body</span></span>
<span data-ttu-id="9223c-128">В тексте запроса добавьте представление объекта Девицеманажементкачедрепортконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9223c-128">In the request body, supply a JSON representation for the deviceManagementCachedReportConfiguration object.</span></span>

<span data-ttu-id="9223c-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкачедрепортконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="9223c-129">The following table shows the properties that are required when you create the deviceManagementCachedReportConfiguration.</span></span>

|<span data-ttu-id="9223c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9223c-130">Property</span></span>|<span data-ttu-id="9223c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9223c-131">Type</span></span>|<span data-ttu-id="9223c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9223c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9223c-133">id</span><span class="sxs-lookup"><span data-stu-id="9223c-133">id</span></span>|<span data-ttu-id="9223c-134">String</span><span class="sxs-lookup"><span data-stu-id="9223c-134">String</span></span>|<span data-ttu-id="9223c-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="9223c-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="9223c-136">репортнаме</span><span class="sxs-lookup"><span data-stu-id="9223c-136">reportName</span></span>|<span data-ttu-id="9223c-137">String</span><span class="sxs-lookup"><span data-stu-id="9223c-137">String</span></span>|<span data-ttu-id="9223c-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="9223c-138">Name of the report</span></span>|
|<span data-ttu-id="9223c-139">filter</span><span class="sxs-lookup"><span data-stu-id="9223c-139">filter</span></span>|<span data-ttu-id="9223c-140">String</span><span class="sxs-lookup"><span data-stu-id="9223c-140">String</span></span>|<span data-ttu-id="9223c-141">Фильтры, применяемые при создании отчета.</span><span class="sxs-lookup"><span data-stu-id="9223c-141">Filters applied on report creation.</span></span>|
|<span data-ttu-id="9223c-142">select</span><span class="sxs-lookup"><span data-stu-id="9223c-142">select</span></span>|<span data-ttu-id="9223c-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9223c-143">String collection</span></span>|<span data-ttu-id="9223c-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="9223c-144">Columns selected from the report</span></span>|
|<span data-ttu-id="9223c-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="9223c-145">orderBy</span></span>|<span data-ttu-id="9223c-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9223c-146">String collection</span></span>|<span data-ttu-id="9223c-147">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="9223c-147">Ordering of columns in the report</span></span>|
|<span data-ttu-id="9223c-148">метаданных</span><span class="sxs-lookup"><span data-stu-id="9223c-148">metadata</span></span>|<span data-ttu-id="9223c-149">String</span><span class="sxs-lookup"><span data-stu-id="9223c-149">String</span></span>|<span data-ttu-id="9223c-150">Управляемые вызывающими метаданными метаданные, связанные с отчетом</span><span class="sxs-lookup"><span data-stu-id="9223c-150">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="9223c-151">status</span><span class="sxs-lookup"><span data-stu-id="9223c-151">status</span></span>|[<span data-ttu-id="9223c-152">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="9223c-152">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="9223c-153">Состояние кэшированного отчета.</span><span class="sxs-lookup"><span data-stu-id="9223c-153">Status of the cached report.</span></span> <span data-ttu-id="9223c-154">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9223c-154">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="9223c-155">ластрефрешдатетиме</span><span class="sxs-lookup"><span data-stu-id="9223c-155">lastRefreshDateTime</span></span>|<span data-ttu-id="9223c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9223c-156">DateTimeOffset</span></span>|<span data-ttu-id="9223c-157">Время последнего обновления кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="9223c-157">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="9223c-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9223c-158">expirationDateTime</span></span>|<span data-ttu-id="9223c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9223c-159">DateTimeOffset</span></span>|<span data-ttu-id="9223c-160">Время истечения срока действия кэшированного отчета</span><span class="sxs-lookup"><span data-stu-id="9223c-160">Time that the cached report expires</span></span>|



## <a name="response"></a><span data-ttu-id="9223c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="9223c-161">Response</span></span>
<span data-ttu-id="9223c-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9223c-162">If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9223c-163">Пример</span><span class="sxs-lookup"><span data-stu-id="9223c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9223c-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="9223c-164">Request</span></span>
<span data-ttu-id="9223c-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9223c-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9223c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9223c-166">Response</span></span>
<span data-ttu-id="9223c-167">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="9223c-167">Here is an example of the response.</span></span> <span data-ttu-id="9223c-168">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="9223c-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9223c-169">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9223c-169">All of the properties will be returned from an actual call.</span></span>
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



