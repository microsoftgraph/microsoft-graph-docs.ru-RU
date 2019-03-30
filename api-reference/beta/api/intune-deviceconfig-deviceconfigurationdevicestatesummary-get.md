---
title: Получение объекта deviceConfigurationDeviceStateSummary
description: Чтение свойств и связей объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2baf921584f8cbcdba0ba734f4f512987e26c725
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989108"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="b0057-103">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b0057-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="b0057-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0057-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0057-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0057-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0057-106">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b0057-106">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0057-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0057-107">Prerequisites</span></span>
<span data-ttu-id="b0057-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0057-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0057-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0057-110">Permission type</span></span>|<span data-ttu-id="b0057-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0057-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0057-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0057-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0057-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0057-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0057-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0057-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0057-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0057-115">Not supported.</span></span>|
|<span data-ttu-id="b0057-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0057-116">Application</span></span>|<span data-ttu-id="b0057-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0057-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0057-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0057-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0057-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0057-119">Optional query parameters</span></span>
<span data-ttu-id="b0057-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0057-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0057-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0057-121">Request headers</span></span>
|<span data-ttu-id="b0057-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0057-122">Header</span></span>|<span data-ttu-id="b0057-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b0057-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0057-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0057-124">Authorization</span></span>|<span data-ttu-id="b0057-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0057-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0057-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b0057-126">Accept</span></span>|<span data-ttu-id="b0057-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0057-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0057-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0057-128">Request body</span></span>
<span data-ttu-id="b0057-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0057-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0057-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0057-130">Response</span></span>
<span data-ttu-id="b0057-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0057-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0057-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0057-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0057-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0057-133">Request</span></span>
<span data-ttu-id="b0057-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0057-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="b0057-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0057-135">Response</span></span>
<span data-ttu-id="b0057-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0057-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
    "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```




