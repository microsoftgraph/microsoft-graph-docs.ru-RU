---
title: Get dataSharingConsent
description: Чтение свойств и связей объекта dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e7e9468da9db40199f77e9a7bdffb7d459a2766
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146561"
---
# <a name="get-datasharingconsent"></a><span data-ttu-id="e2431-103">Get dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="e2431-103">Get dataSharingConsent</span></span>

<span data-ttu-id="e2431-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2431-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2431-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2431-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2431-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2431-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2431-107">Чтение свойств и связей объекта [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="e2431-107">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2431-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2431-108">Prerequisites</span></span>
<span data-ttu-id="e2431-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2431-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2431-111">Permission type</span></span>|<span data-ttu-id="e2431-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2431-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2431-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2431-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2431-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2431-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e2431-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2431-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2431-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2431-116">Not supported.</span></span>|
|<span data-ttu-id="e2431-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e2431-117">Application</span></span>|<span data-ttu-id="e2431-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2431-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2431-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2431-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2431-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2431-120">Optional query parameters</span></span>
<span data-ttu-id="e2431-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2431-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2431-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2431-122">Request headers</span></span>
|<span data-ttu-id="e2431-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2431-123">Header</span></span>|<span data-ttu-id="e2431-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e2431-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2431-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2431-125">Authorization</span></span>|<span data-ttu-id="e2431-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2431-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2431-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e2431-127">Accept</span></span>|<span data-ttu-id="e2431-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2431-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2431-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2431-129">Request body</span></span>
<span data-ttu-id="e2431-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2431-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2431-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2431-131">Response</span></span>
<span data-ttu-id="e2431-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e2431-132">If successful, this method returns a `200 OK` response code and [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2431-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e2431-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2431-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2431-134">Request</span></span>
<span data-ttu-id="e2431-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2431-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

### <a name="response"></a><span data-ttu-id="e2431-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2431-136">Response</span></span>
<span data-ttu-id="e2431-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2431-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```




