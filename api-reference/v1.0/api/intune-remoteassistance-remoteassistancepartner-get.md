---
title: Получение remoteAssistancePartner
description: Чтение свойств и связей объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75531111b9fc6c8bc6571eee5ec3e8e149f5f813
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942138"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="0dbcf-103">Получение remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="0dbcf-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="0dbcf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0dbcf-105">Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="0dbcf-105">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0dbcf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0dbcf-106">Prerequisites</span></span>
<span data-ttu-id="0dbcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dbcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dbcf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dbcf-109">Permission type</span></span>|<span data-ttu-id="0dbcf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dbcf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dbcf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dbcf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0dbcf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0dbcf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0dbcf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dbcf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dbcf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-114">Not supported.</span></span>|
|<span data-ttu-id="0dbcf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0dbcf-115">Application</span></span>|<span data-ttu-id="0dbcf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dbcf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dbcf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0dbcf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0dbcf-118">Optional query parameters</span></span>
<span data-ttu-id="0dbcf-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0dbcf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0dbcf-120">Request headers</span></span>
|<span data-ttu-id="0dbcf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0dbcf-121">Header</span></span>|<span data-ttu-id="0dbcf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0dbcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dbcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dbcf-123">Authorization</span></span>|<span data-ttu-id="0dbcf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0dbcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dbcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0dbcf-125">Accept</span></span>|<span data-ttu-id="0dbcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dbcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dbcf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0dbcf-127">Request body</span></span>
<span data-ttu-id="0dbcf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dbcf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dbcf-129">Response</span></span>
<span data-ttu-id="0dbcf-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-130">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dbcf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0dbcf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0dbcf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dbcf-132">Request</span></span>
<span data-ttu-id="0dbcf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="0dbcf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dbcf-134">Response</span></span>
<span data-ttu-id="0dbcf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0dbcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "onboarding",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



