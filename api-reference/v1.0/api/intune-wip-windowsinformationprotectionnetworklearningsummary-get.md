---
title: Получение windowsInformationProtectionNetworkLearningSummary
description: Чтение свойств и связей объекта windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc5fbd9585c591b4171d7f26c92fca0660e36929
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461127"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="394bb-103">Получение windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="394bb-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="394bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="394bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="394bb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="394bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="394bb-106">Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="394bb-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="394bb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="394bb-107">Prerequisites</span></span>
<span data-ttu-id="394bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="394bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="394bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="394bb-110">Permission type</span></span>|<span data-ttu-id="394bb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="394bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="394bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="394bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="394bb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="394bb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="394bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="394bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="394bb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="394bb-115">Not supported.</span></span>|
|<span data-ttu-id="394bb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="394bb-116">Application</span></span>|<span data-ttu-id="394bb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="394bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="394bb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="394bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="394bb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="394bb-119">Optional query parameters</span></span>
<span data-ttu-id="394bb-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="394bb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="394bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="394bb-121">Request headers</span></span>
|<span data-ttu-id="394bb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="394bb-122">Header</span></span>|<span data-ttu-id="394bb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="394bb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="394bb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="394bb-124">Authorization</span></span>|<span data-ttu-id="394bb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="394bb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="394bb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="394bb-126">Accept</span></span>|<span data-ttu-id="394bb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="394bb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="394bb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="394bb-128">Request body</span></span>
<span data-ttu-id="394bb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="394bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="394bb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="394bb-130">Response</span></span>
<span data-ttu-id="394bb-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="394bb-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="394bb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="394bb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="394bb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="394bb-133">Request</span></span>
<span data-ttu-id="394bb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="394bb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="394bb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="394bb-135">Response</span></span>
<span data-ttu-id="394bb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="394bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






