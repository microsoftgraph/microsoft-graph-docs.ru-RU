---
title: Получение windowsInformationProtectionNetworkLearningSummary
description: Чтение свойств и связей объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9fb911985cf17fbfd8db10a5caf30469a63e082c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960499"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="f4091-103">Получение windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="f4091-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="f4091-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f4091-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4091-105">Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f4091-105">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4091-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4091-106">Prerequisites</span></span>
<span data-ttu-id="f4091-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4091-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4091-109">Permission type</span></span>|<span data-ttu-id="f4091-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4091-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4091-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4091-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4091-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4091-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f4091-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4091-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4091-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4091-114">Not supported.</span></span>|
|<span data-ttu-id="f4091-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4091-115">Application</span></span>|<span data-ttu-id="f4091-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4091-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4091-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4091-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4091-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4091-118">Optional query parameters</span></span>
<span data-ttu-id="f4091-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f4091-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f4091-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4091-120">Request headers</span></span>
|<span data-ttu-id="f4091-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4091-121">Header</span></span>|<span data-ttu-id="f4091-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4091-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4091-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4091-123">Authorization</span></span>|<span data-ttu-id="f4091-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4091-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4091-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4091-125">Accept</span></span>|<span data-ttu-id="f4091-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4091-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4091-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4091-127">Request body</span></span>
<span data-ttu-id="f4091-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4091-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4091-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4091-129">Response</span></span>
<span data-ttu-id="f4091-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4091-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4091-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f4091-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4091-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4091-132">Request</span></span>
<span data-ttu-id="f4091-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4091-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="f4091-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4091-134">Response</span></span>
<span data-ttu-id="f4091-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f4091-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
    "id": "242108f7-08f7-2421-f708-2124f7082124",
    "url": "Url value",
    "deviceCount": 11
  }
}
```



