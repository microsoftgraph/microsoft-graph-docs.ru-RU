---
title: Список Ндесконнекторс
description: Список свойств и связей объектов Ндесконнектор.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 508f4008b2bded53e9cae56f5ae1c5abcf7f22a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314951"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="5a2aa-103">Список Ндесконнекторс</span><span class="sxs-lookup"><span data-stu-id="5a2aa-103">List ndesConnectors</span></span>

> <span data-ttu-id="5a2aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a2aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a2aa-106">Список свойств и связей объектов [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2aa-106">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a2aa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a2aa-107">Prerequisites</span></span>
<span data-ttu-id="5a2aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a2aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a2aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a2aa-110">Permission type</span></span>|<span data-ttu-id="5a2aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a2aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a2aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a2aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a2aa-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a2aa-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a2aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a2aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a2aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-115">Not supported.</span></span>|
|<span data-ttu-id="5a2aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a2aa-116">Application</span></span>|<span data-ttu-id="5a2aa-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a2aa-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a2aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a2aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5a2aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a2aa-119">Request headers</span></span>
|<span data-ttu-id="5a2aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a2aa-120">Header</span></span>|<span data-ttu-id="5a2aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a2aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a2aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a2aa-122">Authorization</span></span>|<span data-ttu-id="5a2aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a2aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a2aa-124">Accept</span></span>|<span data-ttu-id="5a2aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a2aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a2aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a2aa-126">Request body</span></span>
<span data-ttu-id="5a2aa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a2aa-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a2aa-128">Response</span></span>
<span data-ttu-id="5a2aa-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-129">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a2aa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5a2aa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a2aa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a2aa-131">Request</span></span>
<span data-ttu-id="5a2aa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="5a2aa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a2aa-133">Response</span></span>
<span data-ttu-id="5a2aa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a2aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






