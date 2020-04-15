---
title: Получение объекта telecomExpenseManagementPartner
description: Чтение свойств и связей объекта telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56237eded27c2d83b3ff1bfdbbfa180277a69803
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411106"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="92f73-103">Получение объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="92f73-103">Get telecomExpenseManagementPartner</span></span>

<span data-ttu-id="92f73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92f73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92f73-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92f73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92f73-106">Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="92f73-106">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92f73-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="92f73-107">Prerequisites</span></span>
<span data-ttu-id="92f73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92f73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92f73-110">Permission type</span></span>|<span data-ttu-id="92f73-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92f73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92f73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92f73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92f73-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="92f73-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="92f73-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92f73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92f73-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f73-115">Not supported.</span></span>|
|<span data-ttu-id="92f73-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92f73-116">Application</span></span>|<span data-ttu-id="92f73-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92f73-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92f73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92f73-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92f73-119">Optional query parameters</span></span>
<span data-ttu-id="92f73-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92f73-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92f73-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92f73-121">Request headers</span></span>
|<span data-ttu-id="92f73-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92f73-122">Header</span></span>|<span data-ttu-id="92f73-123">Значение</span><span class="sxs-lookup"><span data-stu-id="92f73-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92f73-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="92f73-124">Authorization</span></span>|<span data-ttu-id="92f73-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92f73-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92f73-126">Accept</span><span class="sxs-lookup"><span data-stu-id="92f73-126">Accept</span></span>|<span data-ttu-id="92f73-127">application/json</span><span class="sxs-lookup"><span data-stu-id="92f73-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92f73-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92f73-128">Request body</span></span>
<span data-ttu-id="92f73-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92f73-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92f73-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="92f73-130">Response</span></span>
<span data-ttu-id="92f73-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92f73-131">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92f73-132">Пример</span><span class="sxs-lookup"><span data-stu-id="92f73-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="92f73-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="92f73-133">Request</span></span>
<span data-ttu-id="92f73-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92f73-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="92f73-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="92f73-135">Response</span></span>
<span data-ttu-id="92f73-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92f73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






