---
title: Получение windowsInformationProtectionNetworkLearningSummary
description: Чтение свойств и связей объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 096d3a01cec737f147d907846ca852f4f5b7eba3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990416"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="0fd11-103">Получение windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="0fd11-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="0fd11-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fd11-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fd11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fd11-106">Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0fd11-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fd11-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0fd11-107">Prerequisites</span></span>
<span data-ttu-id="0fd11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fd11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fd11-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fd11-110">Permission type</span></span>|<span data-ttu-id="0fd11-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fd11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fd11-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fd11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fd11-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fd11-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0fd11-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fd11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fd11-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd11-115">Not supported.</span></span>|
|<span data-ttu-id="0fd11-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fd11-116">Application</span></span>|<span data-ttu-id="0fd11-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd11-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fd11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fd11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fd11-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0fd11-119">Optional query parameters</span></span>
<span data-ttu-id="0fd11-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0fd11-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fd11-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fd11-121">Request headers</span></span>
|<span data-ttu-id="0fd11-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fd11-122">Header</span></span>|<span data-ttu-id="0fd11-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0fd11-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fd11-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fd11-124">Authorization</span></span>|<span data-ttu-id="0fd11-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fd11-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fd11-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0fd11-126">Accept</span></span>|<span data-ttu-id="0fd11-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0fd11-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fd11-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fd11-128">Request body</span></span>
<span data-ttu-id="0fd11-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fd11-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fd11-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fd11-130">Response</span></span>
<span data-ttu-id="0fd11-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0fd11-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fd11-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0fd11-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fd11-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fd11-133">Request</span></span>
<span data-ttu-id="0fd11-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fd11-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="0fd11-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fd11-135">Response</span></span>
<span data-ttu-id="0fd11-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fd11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





