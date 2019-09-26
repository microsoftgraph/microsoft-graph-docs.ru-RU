---
title: Получение объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ae6148a7c9e9c66ecd0979c4b5562c4b952c1f7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177383"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="8f782-103">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8f782-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="8f782-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f782-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f782-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f782-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f782-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8f782-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f782-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8f782-107">Prerequisites</span></span>
<span data-ttu-id="8f782-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f782-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f782-110">Permission type</span></span>|<span data-ttu-id="8f782-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f782-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f782-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f782-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f782-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f782-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f782-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f782-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f782-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f782-115">Not supported.</span></span>|
|<span data-ttu-id="8f782-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f782-116">Application</span></span>|<span data-ttu-id="8f782-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f782-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f782-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f782-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f782-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f782-119">Optional query parameters</span></span>
<span data-ttu-id="8f782-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f782-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f782-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f782-121">Request headers</span></span>
|<span data-ttu-id="8f782-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f782-122">Header</span></span>|<span data-ttu-id="8f782-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8f782-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f782-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f782-124">Authorization</span></span>|<span data-ttu-id="8f782-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f782-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f782-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8f782-126">Accept</span></span>|<span data-ttu-id="8f782-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8f782-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f782-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f782-128">Request body</span></span>
<span data-ttu-id="8f782-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f782-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f782-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f782-130">Response</span></span>
<span data-ttu-id="8f782-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f782-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f782-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8f782-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f782-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f782-133">Request</span></span>
<span data-ttu-id="8f782-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f782-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="8f782-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f782-135">Response</span></span>
<span data-ttu-id="8f782-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f782-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```




