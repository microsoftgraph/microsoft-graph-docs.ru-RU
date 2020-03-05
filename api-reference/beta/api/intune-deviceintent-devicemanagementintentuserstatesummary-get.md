---
title: Получение Девицеманажементинтентусерстатесуммари
description: Чтение свойств и связей объекта Девицеманажементинтентусерстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7342908be305616ba8718aa6ce810190a9e154a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470730"
---
# <a name="get-devicemanagementintentuserstatesummary"></a><span data-ttu-id="5104b-103">Получение Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="5104b-103">Get deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="5104b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5104b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5104b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5104b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5104b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5104b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5104b-107">Чтение свойств и связей объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5104b-107">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5104b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5104b-108">Prerequisites</span></span>
<span data-ttu-id="5104b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5104b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5104b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5104b-111">Permission type</span></span>|<span data-ttu-id="5104b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5104b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5104b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5104b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5104b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5104b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5104b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5104b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5104b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5104b-116">Not supported.</span></span>|
|<span data-ttu-id="5104b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5104b-117">Application</span></span>|<span data-ttu-id="5104b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5104b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5104b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5104b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5104b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5104b-120">Optional query parameters</span></span>
<span data-ttu-id="5104b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5104b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5104b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5104b-122">Request headers</span></span>
|<span data-ttu-id="5104b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5104b-123">Header</span></span>|<span data-ttu-id="5104b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5104b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5104b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5104b-125">Authorization</span></span>|<span data-ttu-id="5104b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5104b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5104b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5104b-127">Accept</span></span>|<span data-ttu-id="5104b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5104b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5104b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5104b-129">Request body</span></span>
<span data-ttu-id="5104b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5104b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5104b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5104b-131">Response</span></span>
<span data-ttu-id="5104b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5104b-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5104b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5104b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5104b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5104b-134">Request</span></span>
<span data-ttu-id="5104b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5104b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="5104b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5104b-136">Response</span></span>
<span data-ttu-id="5104b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5104b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
    "id": "be567e02-7e02-be56-027e-56be027e56be",
    "conflictCount": 13,
    "errorCount": 10,
    "failedCount": 11,
    "notApplicableCount": 2,
    "successCount": 12
  }
}
```





