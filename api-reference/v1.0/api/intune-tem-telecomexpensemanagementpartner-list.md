---
title: Список объектов telecomExpenseManagementPartner
description: Список свойств и связей объектов telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f86d5c65bf1a2b6a8d31f347a4797485db0974f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970761"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="553ce-103">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="553ce-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="553ce-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="553ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="553ce-105">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="553ce-105">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="553ce-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="553ce-106">Prerequisites</span></span>
<span data-ttu-id="553ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553ce-109">Permission type</span></span>|<span data-ttu-id="553ce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="553ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="553ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="553ce-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="553ce-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="553ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="553ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553ce-114">Not supported.</span></span>|
|<span data-ttu-id="553ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553ce-115">Application</span></span>|<span data-ttu-id="553ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="553ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="553ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553ce-118">Request headers</span></span>
|<span data-ttu-id="553ce-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="553ce-119">Header</span></span>|<span data-ttu-id="553ce-120">Значение</span><span class="sxs-lookup"><span data-stu-id="553ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="553ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="553ce-121">Authorization</span></span>|<span data-ttu-id="553ce-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="553ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="553ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="553ce-123">Accept</span></span>|<span data-ttu-id="553ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="553ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="553ce-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="553ce-125">Request body</span></span>
<span data-ttu-id="553ce-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="553ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553ce-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="553ce-127">Response</span></span>
<span data-ttu-id="553ce-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="553ce-128">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="553ce-129">Пример</span><span class="sxs-lookup"><span data-stu-id="553ce-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="553ce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="553ce-130">Request</span></span>
<span data-ttu-id="553ce-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="553ce-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="553ce-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="553ce-132">Response</span></span>
<span data-ttu-id="553ce-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="553ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```



