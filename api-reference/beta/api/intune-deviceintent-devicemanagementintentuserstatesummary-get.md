---
title: Получение Девицеманажементинтентусерстатесуммари
description: Чтение свойств и связей объекта Девицеманажементинтентусерстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba0de6c8b53008b12e27e9b2fd9221f8c77d2dda
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945643"
---
# <a name="get-devicemanagementintentuserstatesummary"></a><span data-ttu-id="b0bc1-103">Получение Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="b0bc1-103">Get deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="b0bc1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0bc1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0bc1-106">Чтение свойств и связей объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b0bc1-106">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0bc1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0bc1-107">Prerequisites</span></span>
<span data-ttu-id="b0bc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0bc1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0bc1-110">Permission type</span></span>|<span data-ttu-id="b0bc1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0bc1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0bc1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0bc1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0bc1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0bc1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0bc1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0bc1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0bc1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-115">Not supported.</span></span>|
|<span data-ttu-id="b0bc1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0bc1-116">Application</span></span>|<span data-ttu-id="b0bc1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0bc1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0bc1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0bc1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0bc1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0bc1-119">Optional query parameters</span></span>
<span data-ttu-id="b0bc1-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0bc1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0bc1-121">Request headers</span></span>
|<span data-ttu-id="b0bc1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0bc1-122">Header</span></span>|<span data-ttu-id="b0bc1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b0bc1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0bc1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0bc1-124">Authorization</span></span>|<span data-ttu-id="b0bc1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0bc1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b0bc1-126">Accept</span></span>|<span data-ttu-id="b0bc1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0bc1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0bc1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0bc1-128">Request body</span></span>
<span data-ttu-id="b0bc1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0bc1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0bc1-130">Response</span></span>
<span data-ttu-id="b0bc1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0bc1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0bc1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0bc1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0bc1-133">Request</span></span>
<span data-ttu-id="b0bc1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="b0bc1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0bc1-135">Response</span></span>
<span data-ttu-id="b0bc1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0bc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





