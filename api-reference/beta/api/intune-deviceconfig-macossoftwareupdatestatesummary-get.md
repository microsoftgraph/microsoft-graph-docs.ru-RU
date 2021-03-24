---
title: Get macOSSoftwareUpdateStateSummary
description: Чтение свойств и связей объекта macOSSoftwareUpdateStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b50e852dbacfc9c64eccc7171f8326e8098da2b5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137177"
---
# <a name="get-macossoftwareupdatestatesummary"></a><span data-ttu-id="627ff-103">Get macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="627ff-103">Get macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="627ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="627ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="627ff-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="627ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="627ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="627ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="627ff-107">Чтение свойств и связей объекта [macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="627ff-107">Read properties and relationships of the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="627ff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="627ff-108">Prerequisites</span></span>
<span data-ttu-id="627ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="627ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="627ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="627ff-111">Permission type</span></span>|<span data-ttu-id="627ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="627ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="627ff-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="627ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="627ff-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="627ff-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="627ff-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="627ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="627ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="627ff-116">Not supported.</span></span>|
|<span data-ttu-id="627ff-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="627ff-117">Application</span></span>|<span data-ttu-id="627ff-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="627ff-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="627ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="627ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="627ff-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="627ff-120">Optional query parameters</span></span>
<span data-ttu-id="627ff-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="627ff-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="627ff-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="627ff-122">Request headers</span></span>
|<span data-ttu-id="627ff-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="627ff-123">Header</span></span>|<span data-ttu-id="627ff-124">Значение</span><span class="sxs-lookup"><span data-stu-id="627ff-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="627ff-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="627ff-125">Authorization</span></span>|<span data-ttu-id="627ff-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="627ff-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="627ff-127">Accept</span><span class="sxs-lookup"><span data-stu-id="627ff-127">Accept</span></span>|<span data-ttu-id="627ff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="627ff-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="627ff-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="627ff-129">Request body</span></span>
<span data-ttu-id="627ff-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="627ff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="627ff-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="627ff-131">Response</span></span>
<span data-ttu-id="627ff-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="627ff-132">If successful, this method returns a `200 OK` response code and [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="627ff-133">Пример</span><span class="sxs-lookup"><span data-stu-id="627ff-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="627ff-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="627ff-134">Request</span></span>
<span data-ttu-id="627ff-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="627ff-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="627ff-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="627ff-136">Response</span></span>
<span data-ttu-id="627ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="627ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 415

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
    "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
    "displayName": "Display Name value",
    "productKey": "Product Key value",
    "updateCategory": "configurationDataFile",
    "updateVersion": "Update Version value",
    "state": "downloading",
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```




