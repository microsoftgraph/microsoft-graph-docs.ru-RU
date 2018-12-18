---
title: Получение windowsInformationProtectionNetworkLearningSummary
description: Чтение свойств и связей объекта windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
ms.openlocfilehash: 46c255b5e59ab4245b1945d588bc15b36b55aec8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332132"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="209ed-103">Получение windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="209ed-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="209ed-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="209ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="209ed-105">Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="209ed-105">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="209ed-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="209ed-106">Prerequisites</span></span>
<span data-ttu-id="209ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="209ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="209ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="209ed-109">Permission type</span></span>|<span data-ttu-id="209ed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="209ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="209ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="209ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="209ed-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="209ed-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="209ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="209ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="209ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="209ed-114">Not supported.</span></span>|
|<span data-ttu-id="209ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="209ed-115">Application</span></span>|<span data-ttu-id="209ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="209ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="209ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="209ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="209ed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="209ed-118">Optional query parameters</span></span>
<span data-ttu-id="209ed-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="209ed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="209ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="209ed-120">Request headers</span></span>
|<span data-ttu-id="209ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="209ed-121">Header</span></span>|<span data-ttu-id="209ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="209ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="209ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="209ed-123">Authorization</span></span>|<span data-ttu-id="209ed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="209ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="209ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="209ed-125">Accept</span></span>|<span data-ttu-id="209ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="209ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="209ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="209ed-127">Request body</span></span>
<span data-ttu-id="209ed-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="209ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="209ed-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="209ed-129">Response</span></span>
<span data-ttu-id="209ed-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="209ed-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="209ed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="209ed-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="209ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="209ed-132">Request</span></span>
<span data-ttu-id="209ed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="209ed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="209ed-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="209ed-134">Response</span></span>
<span data-ttu-id="209ed-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="209ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



