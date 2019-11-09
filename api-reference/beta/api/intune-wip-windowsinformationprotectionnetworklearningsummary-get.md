---
title: Получение windowsInformationProtectionNetworkLearningSummary
description: Чтение свойств и связей объекта windowsInformationProtectionNetworkLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5f2b7cac1f7813fc2a61af26b0c9d964726f77b
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087918"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="ebf6f-103">Получение windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="ebf6f-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="ebf6f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebf6f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebf6f-106">Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ebf6f-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebf6f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ebf6f-107">Prerequisites</span></span>
<span data-ttu-id="ebf6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebf6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebf6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebf6f-110">Permission type</span></span>|<span data-ttu-id="ebf6f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebf6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebf6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebf6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebf6f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ebf6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebf6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebf6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-115">Not supported.</span></span>|
|<span data-ttu-id="ebf6f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebf6f-116">Application</span></span>|<span data-ttu-id="ebf6f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebf6f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebf6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebf6f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebf6f-119">Optional query parameters</span></span>
<span data-ttu-id="ebf6f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebf6f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebf6f-121">Request headers</span></span>
|<span data-ttu-id="ebf6f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebf6f-122">Header</span></span>|<span data-ttu-id="ebf6f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ebf6f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebf6f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebf6f-124">Authorization</span></span>|<span data-ttu-id="ebf6f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebf6f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ebf6f-126">Accept</span></span>|<span data-ttu-id="ebf6f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ebf6f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebf6f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebf6f-128">Request body</span></span>
<span data-ttu-id="ebf6f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebf6f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebf6f-130">Response</span></span>
<span data-ttu-id="ebf6f-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebf6f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ebf6f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebf6f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebf6f-133">Request</span></span>
<span data-ttu-id="ebf6f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="ebf6f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebf6f-135">Response</span></span>
<span data-ttu-id="ebf6f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebf6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






