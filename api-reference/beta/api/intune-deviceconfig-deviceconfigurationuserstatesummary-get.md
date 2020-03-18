---
title: Получение Девицеконфигуратионусерстатесуммари
description: Чтение свойств и связей объекта Девицеконфигуратионусерстатесуммари.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb37fe92fdcc919701842cc9fdc8eeb5a9912372
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42753539"
---
# <a name="get-deviceconfigurationuserstatesummary"></a><span data-ttu-id="22828-103">Получение Девицеконфигуратионусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="22828-103">Get deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="22828-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22828-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22828-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22828-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22828-106">Чтение свойств и связей объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="22828-106">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22828-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22828-107">Prerequisites</span></span>
<span data-ttu-id="22828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22828-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22828-110">Permission type</span></span>|<span data-ttu-id="22828-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22828-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22828-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22828-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22828-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22828-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22828-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22828-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22828-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22828-115">Not supported.</span></span>|
|<span data-ttu-id="22828-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="22828-116">Application</span></span>|<span data-ttu-id="22828-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22828-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22828-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22828-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22828-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22828-119">Optional query parameters</span></span>
<span data-ttu-id="22828-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22828-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22828-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22828-121">Request headers</span></span>
|<span data-ttu-id="22828-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22828-122">Header</span></span>|<span data-ttu-id="22828-123">Значение</span><span class="sxs-lookup"><span data-stu-id="22828-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22828-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22828-124">Authorization</span></span>|<span data-ttu-id="22828-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22828-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22828-126">Accept</span><span class="sxs-lookup"><span data-stu-id="22828-126">Accept</span></span>|<span data-ttu-id="22828-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22828-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22828-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22828-128">Request body</span></span>
<span data-ttu-id="22828-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22828-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22828-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="22828-130">Response</span></span>
<span data-ttu-id="22828-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22828-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22828-132">Пример</span><span class="sxs-lookup"><span data-stu-id="22828-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22828-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="22828-133">Request</span></span>
<span data-ttu-id="22828-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22828-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
```

### <a name="response"></a><span data-ttu-id="22828-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="22828-135">Response</span></span>
<span data-ttu-id="22828-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22828-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 361

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
    "id": "e8957887-7887-e895-8778-95e8877895e8",
    "unknownUserCount": 0,
    "notApplicableUserCount": 6,
    "compliantUserCount": 2,
    "remediatedUserCount": 3,
    "nonCompliantUserCount": 5,
    "errorUserCount": 14,
    "conflictUserCount": 1
  }
}
```




