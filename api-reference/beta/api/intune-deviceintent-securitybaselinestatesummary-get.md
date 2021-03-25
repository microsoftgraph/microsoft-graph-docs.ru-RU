---
title: Получить securityBaselineStateSummary
description: Чтение свойств и связей объекта securityBaselineStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4963475b83cb93ccfe8c8c15b5b12cef349c0267
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154513"
---
# <a name="get-securitybaselinestatesummary"></a><span data-ttu-id="7ffd7-103">Получить securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ffd7-103">Get securityBaselineStateSummary</span></span>

<span data-ttu-id="7ffd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ffd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ffd7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ffd7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ffd7-107">Чтение свойств и связей объекта [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="7ffd7-107">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ffd7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7ffd7-108">Prerequisites</span></span>
<span data-ttu-id="7ffd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ffd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ffd7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ffd7-111">Permission type</span></span>|<span data-ttu-id="7ffd7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ffd7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ffd7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ffd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ffd7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffd7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ffd7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ffd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ffd7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-116">Not supported.</span></span>|
|<span data-ttu-id="7ffd7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ffd7-117">Application</span></span>|<span data-ttu-id="7ffd7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffd7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ffd7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ffd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ffd7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ffd7-120">Optional query parameters</span></span>
<span data-ttu-id="7ffd7-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ffd7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ffd7-122">Request headers</span></span>
|<span data-ttu-id="7ffd7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ffd7-123">Header</span></span>|<span data-ttu-id="7ffd7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7ffd7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ffd7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ffd7-125">Authorization</span></span>|<span data-ttu-id="7ffd7-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ffd7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7ffd7-127">Accept</span></span>|<span data-ttu-id="7ffd7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7ffd7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ffd7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ffd7-129">Request body</span></span>
<span data-ttu-id="7ffd7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ffd7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ffd7-131">Response</span></span>
<span data-ttu-id="7ffd7-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-132">If successful, this method returns a `200 OK` response code and [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ffd7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7ffd7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ffd7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ffd7-134">Request</span></span>
<span data-ttu-id="7ffd7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

### <a name="response"></a><span data-ttu-id="7ffd7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ffd7-136">Response</span></span>
<span data-ttu-id="7ffd7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ffd7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
    "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
    "secureCount": 11,
    "notSecureCount": 14,
    "unknownCount": 12,
    "errorCount": 10,
    "conflictCount": 13,
    "notApplicableCount": 2
  }
}
```




