---
title: Получение объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
ms.openlocfilehash: c435fcb8c91b540fc8fa07b1ee9660bf193b7bc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306036"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="45422-103">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="45422-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="45422-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45422-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45422-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45422-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45422-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45422-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45422-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="45422-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45422-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45422-108">Prerequisites</span></span>
<span data-ttu-id="45422-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45422-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45422-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45422-111">Permission type</span></span>|<span data-ttu-id="45422-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45422-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45422-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45422-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45422-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45422-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45422-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45422-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45422-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45422-116">Not supported.</span></span>|
|<span data-ttu-id="45422-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45422-117">Application</span></span>|<span data-ttu-id="45422-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45422-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45422-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45422-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45422-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45422-120">Optional query parameters</span></span>
<span data-ttu-id="45422-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45422-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45422-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45422-122">Request headers</span></span>
|<span data-ttu-id="45422-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45422-123">Header</span></span>|<span data-ttu-id="45422-124">Значение</span><span class="sxs-lookup"><span data-stu-id="45422-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45422-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45422-125">Authorization</span></span>|<span data-ttu-id="45422-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45422-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45422-127">Accept</span><span class="sxs-lookup"><span data-stu-id="45422-127">Accept</span></span>|<span data-ttu-id="45422-128">application/json</span><span class="sxs-lookup"><span data-stu-id="45422-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45422-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45422-129">Request body</span></span>
<span data-ttu-id="45422-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45422-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45422-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="45422-131">Response</span></span>
<span data-ttu-id="45422-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45422-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45422-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45422-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="45422-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45422-134">Request</span></span>
<span data-ttu-id="45422-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45422-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="45422-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="45422-136">Response</span></span>
<span data-ttu-id="45422-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45422-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





