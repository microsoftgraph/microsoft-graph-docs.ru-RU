---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6e21d6071ad08da63d0df839808d12b9bf288887
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853454"
---
# <a name="get-reportroot"></a><span data-ttu-id="5c5f3-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="5c5f3-103">Get reportRoot</span></span>

> <span data-ttu-id="5c5f3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c5f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c5f3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c5f3-107">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="5c5f3-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c5f3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5f3-108">Prerequisites</span></span>
<span data-ttu-id="5c5f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5f3-111">Permission type</span></span>|<span data-ttu-id="5c5f3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c5f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c5f3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c5f3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5c5f3-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="5c5f3-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5c5f3-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c5f3-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5c5f3-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="5c5f3-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5c5f3-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c5f3-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5c5f3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c5f3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c5f3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-119">Not supported.</span></span>|
|<span data-ttu-id="5c5f3-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c5f3-120">Application</span></span>|<span data-ttu-id="5c5f3-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c5f3-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c5f3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c5f3-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c5f3-123">Optional query parameters</span></span>
<span data-ttu-id="5c5f3-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c5f3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c5f3-125">Request headers</span></span>
|<span data-ttu-id="5c5f3-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c5f3-126">Header</span></span>|<span data-ttu-id="5c5f3-127">Значение</span><span class="sxs-lookup"><span data-stu-id="5c5f3-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c5f3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c5f3-128">Authorization</span></span>|<span data-ttu-id="5c5f3-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c5f3-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c5f3-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5c5f3-130">Accept</span></span>|<span data-ttu-id="5c5f3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5c5f3-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5f3-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c5f3-132">Request body</span></span>
<span data-ttu-id="5c5f3-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c5f3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c5f3-134">Response</span></span>
<span data-ttu-id="5c5f3-135">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c5f3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5c5f3-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c5f3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c5f3-137">Request</span></span>
<span data-ttu-id="5c5f3-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="5c5f3-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c5f3-139">Response</span></span>
<span data-ttu-id="5c5f3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c5f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```



