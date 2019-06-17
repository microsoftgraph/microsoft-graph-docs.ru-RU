---
title: Получение Секуритибаселинедевицестате
description: Чтение свойств и связей объекта Секуритибаселинедевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 372aeefd9e658b2f4df2b201adf15373167ee428
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959532"
---
# <a name="get-securitybaselinedevicestate"></a><span data-ttu-id="5424b-103">Получение Секуритибаселинедевицестате</span><span class="sxs-lookup"><span data-stu-id="5424b-103">Get securityBaselineDeviceState</span></span>

> <span data-ttu-id="5424b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5424b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5424b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5424b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5424b-106">Чтение свойств и связей объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="5424b-106">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5424b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5424b-107">Prerequisites</span></span>
<span data-ttu-id="5424b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5424b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5424b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5424b-110">Permission type</span></span>|<span data-ttu-id="5424b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5424b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5424b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5424b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5424b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5424b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5424b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5424b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5424b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5424b-115">Not supported.</span></span>|
|<span data-ttu-id="5424b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5424b-116">Application</span></span>|<span data-ttu-id="5424b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5424b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5424b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5424b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5424b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5424b-119">Optional query parameters</span></span>
<span data-ttu-id="5424b-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5424b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5424b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5424b-121">Request headers</span></span>
|<span data-ttu-id="5424b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5424b-122">Header</span></span>|<span data-ttu-id="5424b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5424b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5424b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5424b-124">Authorization</span></span>|<span data-ttu-id="5424b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5424b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5424b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5424b-126">Accept</span></span>|<span data-ttu-id="5424b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5424b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5424b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5424b-128">Request body</span></span>
<span data-ttu-id="5424b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5424b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5424b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5424b-130">Response</span></span>
<span data-ttu-id="5424b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5424b-131">If successful, this method returns a `200 OK` response code and [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5424b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5424b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5424b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5424b-133">Request</span></span>
<span data-ttu-id="5424b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5424b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="5424b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5424b-135">Response</span></span>
<span data-ttu-id="5424b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5424b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
    "id": "182749bf-49bf-1827-bf49-2718bf492718",
    "managedDeviceId": "Managed Device Id value",
    "deviceDisplayName": "Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "state": "secure",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```





