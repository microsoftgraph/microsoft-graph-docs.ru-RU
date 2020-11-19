---
title: Список Макоссофтвареупдатестатесуммариес
description: Список свойств и связей объектов Макоссофтвареупдатестатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 075e1b96db819072b557e14f5f51fc6eb3f9386e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219862"
---
# <a name="list-macossoftwareupdatestatesummaries"></a><span data-ttu-id="311fa-103">Список Макоссофтвареупдатестатесуммариес</span><span class="sxs-lookup"><span data-stu-id="311fa-103">List macOSSoftwareUpdateStateSummaries</span></span>

<span data-ttu-id="311fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="311fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="311fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="311fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="311fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="311fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="311fa-107">Список свойств и связей объектов [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="311fa-107">List properties and relationships of the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="311fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="311fa-108">Prerequisites</span></span>
<span data-ttu-id="311fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="311fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="311fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="311fa-111">Permission type</span></span>|<span data-ttu-id="311fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="311fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="311fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="311fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="311fa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="311fa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="311fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="311fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="311fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="311fa-116">Not supported.</span></span>|
|<span data-ttu-id="311fa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="311fa-117">Application</span></span>|<span data-ttu-id="311fa-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="311fa-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="311fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="311fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="311fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="311fa-120">Request headers</span></span>
|<span data-ttu-id="311fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="311fa-121">Header</span></span>|<span data-ttu-id="311fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="311fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="311fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="311fa-123">Authorization</span></span>|<span data-ttu-id="311fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="311fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="311fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="311fa-125">Accept</span></span>|<span data-ttu-id="311fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="311fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="311fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="311fa-127">Request body</span></span>
<span data-ttu-id="311fa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="311fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="311fa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="311fa-129">Response</span></span>
<span data-ttu-id="311fa-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="311fa-130">If successful, this method returns a `200 OK` response code and a collection of [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="311fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="311fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="311fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="311fa-132">Request</span></span>
<span data-ttu-id="311fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="311fa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
```

### <a name="response"></a><span data-ttu-id="311fa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="311fa-134">Response</span></span>
<span data-ttu-id="311fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="311fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
      "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
      "displayName": "Display Name value",
      "productKey": "Product Key value",
      "updateCategory": "configurationDataFile",
      "updateVersion": "Update Version value",
      "state": "downloading",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




