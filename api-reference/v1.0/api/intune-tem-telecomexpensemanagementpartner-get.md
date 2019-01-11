---
title: Получение объекта telecomExpenseManagementPartner
description: Чтение свойств и связей объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba9e9933424bd63277ecc80acf3d3aaecdd7e4ee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818160"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="ee0fc-103">Получение объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ee0fc-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="ee0fc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee0fc-105">Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="ee0fc-105">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee0fc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee0fc-106">Prerequisites</span></span>
<span data-ttu-id="ee0fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0fc-109">Permission type</span></span>|<span data-ttu-id="ee0fc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee0fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee0fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee0fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee0fc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee0fc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ee0fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee0fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee0fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-114">Not supported.</span></span>|
|<span data-ttu-id="ee0fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee0fc-115">Application</span></span>|<span data-ttu-id="ee0fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee0fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee0fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee0fc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee0fc-118">Optional query parameters</span></span>
<span data-ttu-id="ee0fc-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ee0fc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee0fc-120">Request headers</span></span>
|<span data-ttu-id="ee0fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee0fc-121">Header</span></span>|<span data-ttu-id="ee0fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee0fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee0fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee0fc-123">Authorization</span></span>|<span data-ttu-id="ee0fc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ee0fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee0fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee0fc-125">Accept</span></span>|<span data-ttu-id="ee0fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee0fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0fc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee0fc-127">Request body</span></span>
<span data-ttu-id="ee0fc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee0fc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0fc-129">Response</span></span>
<span data-ttu-id="ee0fc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-130">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee0fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ee0fc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee0fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee0fc-132">Request</span></span>
<span data-ttu-id="ee0fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="ee0fc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee0fc-134">Response</span></span>
<span data-ttu-id="ee0fc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee0fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



