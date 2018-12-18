---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: tfitzmac
ms.openlocfilehash: aa79d3bbc03529c20e0ea66b91c89a92f7782b2d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339412"
---
# <a name="get-reportroot"></a><span data-ttu-id="08ae0-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="08ae0-103">Get reportRoot</span></span>

> <span data-ttu-id="08ae0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08ae0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08ae0-105">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="08ae0-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08ae0-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="08ae0-106">Prerequisites</span></span>
<span data-ttu-id="08ae0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ae0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08ae0-109">Permission type</span></span>|<span data-ttu-id="08ae0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08ae0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08ae0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08ae0-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="08ae0-112">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="08ae0-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="08ae0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08ae0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="08ae0-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="08ae0-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="08ae0-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="08ae0-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="08ae0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08ae0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08ae0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ae0-117">Not supported.</span></span>|
|<span data-ttu-id="08ae0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08ae0-118">Application</span></span>|<span data-ttu-id="08ae0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ae0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08ae0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08ae0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08ae0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08ae0-121">Optional query parameters</span></span>
<span data-ttu-id="08ae0-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08ae0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08ae0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08ae0-123">Request headers</span></span>
|<span data-ttu-id="08ae0-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08ae0-124">Header</span></span>|<span data-ttu-id="08ae0-125">Значение</span><span class="sxs-lookup"><span data-stu-id="08ae0-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08ae0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08ae0-126">Authorization</span></span>|<span data-ttu-id="08ae0-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="08ae0-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08ae0-128">Accept</span><span class="sxs-lookup"><span data-stu-id="08ae0-128">Accept</span></span>|<span data-ttu-id="08ae0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="08ae0-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ae0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08ae0-130">Request body</span></span>
<span data-ttu-id="08ae0-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08ae0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ae0-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="08ae0-132">Response</span></span>
<span data-ttu-id="08ae0-133">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08ae0-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08ae0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="08ae0-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="08ae0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="08ae0-135">Request</span></span>
<span data-ttu-id="08ae0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08ae0-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="08ae0-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="08ae0-137">Response</span></span>
<span data-ttu-id="08ae0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08ae0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








