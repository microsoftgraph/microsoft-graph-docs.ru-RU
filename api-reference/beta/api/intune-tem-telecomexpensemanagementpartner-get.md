---
title: Получение объекта telecomExpenseManagementPartner
description: Чтение свойств и связей объекта telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b3deff4cf97d036ae889241306cca77b4a7eef9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851935"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="18f76-103">Получение объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="18f76-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="18f76-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18f76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18f76-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18f76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18f76-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18f76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18f76-107">Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="18f76-107">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18f76-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="18f76-108">Prerequisites</span></span>
<span data-ttu-id="18f76-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18f76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18f76-111">Permission type</span></span>|<span data-ttu-id="18f76-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18f76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18f76-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18f76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18f76-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="18f76-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="18f76-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18f76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18f76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18f76-116">Not supported.</span></span>|
|<span data-ttu-id="18f76-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18f76-117">Application</span></span>|<span data-ttu-id="18f76-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18f76-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18f76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18f76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18f76-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18f76-120">Optional query parameters</span></span>
<span data-ttu-id="18f76-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18f76-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="18f76-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18f76-122">Request headers</span></span>
|<span data-ttu-id="18f76-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18f76-123">Header</span></span>|<span data-ttu-id="18f76-124">Значение</span><span class="sxs-lookup"><span data-stu-id="18f76-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18f76-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f76-125">Authorization</span></span>|<span data-ttu-id="18f76-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18f76-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18f76-127">Accept</span><span class="sxs-lookup"><span data-stu-id="18f76-127">Accept</span></span>|<span data-ttu-id="18f76-128">application/json</span><span class="sxs-lookup"><span data-stu-id="18f76-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18f76-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18f76-129">Request body</span></span>
<span data-ttu-id="18f76-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18f76-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18f76-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="18f76-131">Response</span></span>
<span data-ttu-id="18f76-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18f76-132">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f76-133">Пример</span><span class="sxs-lookup"><span data-stu-id="18f76-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="18f76-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="18f76-134">Request</span></span>
<span data-ttu-id="18f76-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18f76-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="18f76-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="18f76-136">Response</span></span>
<span data-ttu-id="18f76-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18f76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





