---
title: Get deviceConfigurationUserOverview
description: Чтение свойств и связей объекта deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01b278e94160d2f64ab97838aa48cb285e61c7a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255761"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="35f0d-103">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="35f0d-103">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="35f0d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35f0d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f0d-105">Чтение свойств и связей объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="35f0d-105">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f0d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="35f0d-106">Prerequisites</span></span>
<span data-ttu-id="35f0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="35f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="35f0d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35f0d-109">Permission type</span></span>|<span data-ttu-id="35f0d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35f0d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f0d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35f0d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35f0d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35f0d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="35f0d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35f0d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f0d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f0d-114">Not supported.</span></span>|
|<span data-ttu-id="35f0d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35f0d-115">Application</span></span>|<span data-ttu-id="35f0d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f0d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f0d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35f0d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35f0d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35f0d-118">Optional query parameters</span></span>
<span data-ttu-id="35f0d-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35f0d-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35f0d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35f0d-120">Request headers</span></span>
|<span data-ttu-id="35f0d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35f0d-121">Header</span></span>|<span data-ttu-id="35f0d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35f0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35f0d-123">Authorization</span></span>|<span data-ttu-id="35f0d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35f0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f0d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35f0d-125">Accept</span></span>|<span data-ttu-id="35f0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35f0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f0d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35f0d-127">Request body</span></span>
<span data-ttu-id="35f0d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35f0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35f0d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="35f0d-129">Response</span></span>
<span data-ttu-id="35f0d-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="35f0d-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f0d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35f0d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f0d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35f0d-132">Request</span></span>
<span data-ttu-id="35f0d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35f0d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="35f0d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="35f0d-134">Response</span></span>
<span data-ttu-id="35f0d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35f0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 368

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



