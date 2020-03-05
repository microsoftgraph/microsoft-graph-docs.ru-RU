---
title: Получение Ндесконнектор
description: Чтение свойств и связей объекта Ндесконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3106e5499e05338946cf453de3b44f91c1a38fc1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442063"
---
# <a name="get-ndesconnector"></a><span data-ttu-id="92b0f-103">Получение Ндесконнектор</span><span class="sxs-lookup"><span data-stu-id="92b0f-103">Get ndesConnector</span></span>

<span data-ttu-id="92b0f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92b0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92b0f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92b0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92b0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92b0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b0f-107">Чтение свойств и связей объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="92b0f-107">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92b0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92b0f-108">Prerequisites</span></span>
<span data-ttu-id="92b0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92b0f-111">Permission type</span></span>|<span data-ttu-id="92b0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92b0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92b0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92b0f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b0f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92b0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92b0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92b0f-116">Not supported.</span></span>|
|<span data-ttu-id="92b0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92b0f-117">Application</span></span>|<span data-ttu-id="92b0f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b0f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92b0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92b0f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92b0f-120">Optional query parameters</span></span>
<span data-ttu-id="92b0f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92b0f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92b0f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92b0f-122">Request headers</span></span>
|<span data-ttu-id="92b0f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92b0f-123">Header</span></span>|<span data-ttu-id="92b0f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="92b0f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b0f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="92b0f-125">Authorization</span></span>|<span data-ttu-id="92b0f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92b0f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b0f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="92b0f-127">Accept</span></span>|<span data-ttu-id="92b0f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92b0f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b0f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92b0f-129">Request body</span></span>
<span data-ttu-id="92b0f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92b0f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b0f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="92b0f-131">Response</span></span>
<span data-ttu-id="92b0f-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92b0f-132">If successful, this method returns a `200 OK` response code and [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b0f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="92b0f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="92b0f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b0f-134">Request</span></span>
<span data-ttu-id="92b0f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b0f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
```

### <a name="response"></a><span data-ttu-id="92b0f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b0f-136">Response</span></span>
<span data-ttu-id="92b0f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92b0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.ndesConnector",
    "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
    "state": "active",
    "displayName": "Display Name value"
  }
}
```





