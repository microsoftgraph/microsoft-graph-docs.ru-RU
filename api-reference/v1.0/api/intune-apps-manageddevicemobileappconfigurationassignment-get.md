---
title: Get managedDeviceMobileAppConfigurationAssignment
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fbfa4262c82b58dbe913010e18f4eb854e4f2d59
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358629"
---
# <a name="get-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="06cc0-103">Get managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="06cc0-103">Get managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="06cc0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06cc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06cc0-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06cc0-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06cc0-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="06cc0-106">Prerequisites</span></span>
<span data-ttu-id="06cc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06cc0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06cc0-109">Permission type</span></span>|<span data-ttu-id="06cc0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06cc0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06cc0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06cc0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06cc0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06cc0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="06cc0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06cc0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06cc0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06cc0-114">Not supported.</span></span>|
|<span data-ttu-id="06cc0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06cc0-115">Application</span></span>|<span data-ttu-id="06cc0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06cc0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06cc0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06cc0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06cc0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06cc0-118">Optional query parameters</span></span>
<span data-ttu-id="06cc0-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06cc0-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06cc0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06cc0-120">Request headers</span></span>
|<span data-ttu-id="06cc0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06cc0-121">Header</span></span>|<span data-ttu-id="06cc0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06cc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06cc0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06cc0-123">Authorization</span></span>|<span data-ttu-id="06cc0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06cc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06cc0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06cc0-125">Accept</span></span>|<span data-ttu-id="06cc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06cc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06cc0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06cc0-127">Request body</span></span>
<span data-ttu-id="06cc0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06cc0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06cc0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="06cc0-129">Response</span></span>
<span data-ttu-id="06cc0-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06cc0-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06cc0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="06cc0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="06cc0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06cc0-132">Request</span></span>
<span data-ttu-id="06cc0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06cc0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="06cc0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="06cc0-134">Response</span></span>
<span data-ttu-id="06cc0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06cc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
    "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




