---
title: Список Ндесконнекторс
description: Список свойств и связей объектов Ндесконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac49bbf813fe31479d8c14fb8676aee9b7caee57
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442036"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="0f140-103">Список Ндесконнекторс</span><span class="sxs-lookup"><span data-stu-id="0f140-103">List ndesConnectors</span></span>

<span data-ttu-id="0f140-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0f140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f140-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f140-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f140-107">Список свойств и связей объектов [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="0f140-107">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f140-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0f140-108">Prerequisites</span></span>
<span data-ttu-id="0f140-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f140-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f140-111">Permission type</span></span>|<span data-ttu-id="0f140-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f140-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f140-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f140-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f140-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f140-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f140-116">Not supported.</span></span>|
|<span data-ttu-id="0f140-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f140-117">Application</span></span>|<span data-ttu-id="0f140-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f140-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f140-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="0f140-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0f140-120">Request headers</span></span>
|<span data-ttu-id="0f140-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f140-121">Header</span></span>|<span data-ttu-id="0f140-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0f140-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f140-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f140-123">Authorization</span></span>|<span data-ttu-id="0f140-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f140-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f140-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f140-125">Accept</span></span>|<span data-ttu-id="0f140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f140-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f140-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f140-127">Request body</span></span>
<span data-ttu-id="0f140-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f140-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f140-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f140-129">Response</span></span>
<span data-ttu-id="0f140-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f140-130">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f140-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0f140-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f140-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f140-132">Request</span></span>
<span data-ttu-id="0f140-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f140-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="0f140-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f140-134">Response</span></span>
<span data-ttu-id="0f140-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ndesConnector",
      "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "active",
      "displayName": "Display Name value"
    }
  ]
}
```





