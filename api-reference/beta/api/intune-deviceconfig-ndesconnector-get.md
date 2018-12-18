---
title: Получение ndesConnector
description: Чтение свойства и связи объекта ndesConnector.
author: tfitzmac
ms.openlocfilehash: ccff6dd13e37ccee19b9f86b91adcf2f6bbc9960
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352796"
---
# <a name="get-ndesconnector"></a><span data-ttu-id="7a6c4-103">Получение ndesConnector</span><span class="sxs-lookup"><span data-stu-id="7a6c4-103">Get ndesConnector</span></span>

> <span data-ttu-id="7a6c4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a6c4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a6c4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a6c4-107">Чтение свойства и связи объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="7a6c4-107">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a6c4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a6c4-108">Prerequisites</span></span>
<span data-ttu-id="7a6c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a6c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a6c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a6c4-111">Permission type</span></span>|<span data-ttu-id="7a6c4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a6c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a6c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a6c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a6c4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a6c4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a6c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a6c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a6c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-116">Not supported.</span></span>|
|<span data-ttu-id="7a6c4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a6c4-117">Application</span></span>|<span data-ttu-id="7a6c4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a6c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a6c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a6c4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a6c4-120">Optional query parameters</span></span>
<span data-ttu-id="7a6c4-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a6c4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a6c4-122">Request headers</span></span>
|<span data-ttu-id="7a6c4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a6c4-123">Header</span></span>|<span data-ttu-id="7a6c4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7a6c4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a6c4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a6c4-125">Authorization</span></span>|<span data-ttu-id="7a6c4-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7a6c4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a6c4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7a6c4-127">Accept</span></span>|<span data-ttu-id="7a6c4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7a6c4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a6c4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a6c4-129">Request body</span></span>
<span data-ttu-id="7a6c4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a6c4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a6c4-131">Response</span></span>
<span data-ttu-id="7a6c4-132">Успешно завершена, этот метод возвращает `200 OK` объект [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-132">If successful, this method returns a `200 OK` response code and [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a6c4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7a6c4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a6c4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a6c4-134">Request</span></span>
<span data-ttu-id="7a6c4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
```

### <a name="response"></a><span data-ttu-id="7a6c4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a6c4-136">Response</span></span>
<span data-ttu-id="7a6c4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7a6c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





