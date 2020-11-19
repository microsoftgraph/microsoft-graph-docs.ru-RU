---
title: Получение Девицеконфигуратионусерстатесуммари
description: Чтение свойств и связей объекта Девицеконфигуратионусерстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9019c9ab59bdd1a1f7ec21d987032410a7e8e15d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291487"
---
# <a name="get-deviceconfigurationuserstatesummary"></a><span data-ttu-id="78ad0-103">Получение Девицеконфигуратионусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="78ad0-103">Get deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="78ad0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78ad0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78ad0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78ad0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78ad0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78ad0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78ad0-107">Чтение свойств и связей объекта [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="78ad0-107">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78ad0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78ad0-108">Prerequisites</span></span>
<span data-ttu-id="78ad0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78ad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78ad0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78ad0-111">Permission type</span></span>|<span data-ttu-id="78ad0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78ad0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78ad0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78ad0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78ad0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78ad0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78ad0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78ad0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78ad0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78ad0-116">Not supported.</span></span>|
|<span data-ttu-id="78ad0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78ad0-117">Application</span></span>|<span data-ttu-id="78ad0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78ad0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78ad0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78ad0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78ad0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78ad0-120">Optional query parameters</span></span>
<span data-ttu-id="78ad0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="78ad0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78ad0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78ad0-122">Request headers</span></span>
|<span data-ttu-id="78ad0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78ad0-123">Header</span></span>|<span data-ttu-id="78ad0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="78ad0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78ad0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78ad0-125">Authorization</span></span>|<span data-ttu-id="78ad0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78ad0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78ad0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="78ad0-127">Accept</span></span>|<span data-ttu-id="78ad0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="78ad0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78ad0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78ad0-129">Request body</span></span>
<span data-ttu-id="78ad0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78ad0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78ad0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="78ad0-131">Response</span></span>
<span data-ttu-id="78ad0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеконфигуратионусерстатесуммари](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78ad0-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78ad0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="78ad0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="78ad0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="78ad0-134">Request</span></span>
<span data-ttu-id="78ad0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78ad0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
```

### <a name="response"></a><span data-ttu-id="78ad0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="78ad0-136">Response</span></span>
<span data-ttu-id="78ad0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78ad0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




