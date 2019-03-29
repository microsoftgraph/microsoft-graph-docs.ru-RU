---
title: Get deviceConfigurationUserOverview
description: Чтение свойств и связей объекта deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67bffb351e6019d1987bee5e39fefdad77036132
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977501"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="55951-103">Get deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="55951-103">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="55951-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55951-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55951-105">Чтение свойств и связей объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="55951-105">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55951-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="55951-106">Prerequisites</span></span>
<span data-ttu-id="55951-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55951-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55951-109">Permission type</span></span>|<span data-ttu-id="55951-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55951-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55951-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55951-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55951-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55951-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55951-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55951-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55951-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55951-114">Not supported.</span></span>|
|<span data-ttu-id="55951-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55951-115">Application</span></span>|<span data-ttu-id="55951-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55951-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55951-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55951-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55951-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55951-118">Optional query parameters</span></span>
<span data-ttu-id="55951-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55951-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55951-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55951-120">Request headers</span></span>
|<span data-ttu-id="55951-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55951-121">Header</span></span>|<span data-ttu-id="55951-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55951-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55951-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55951-123">Authorization</span></span>|<span data-ttu-id="55951-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55951-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55951-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55951-125">Accept</span></span>|<span data-ttu-id="55951-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55951-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55951-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55951-127">Request body</span></span>
<span data-ttu-id="55951-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55951-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55951-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="55951-129">Response</span></span>
<span data-ttu-id="55951-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55951-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55951-131">Пример</span><span class="sxs-lookup"><span data-stu-id="55951-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="55951-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="55951-132">Request</span></span>
<span data-ttu-id="55951-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55951-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="55951-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="55951-134">Response</span></span>
<span data-ttu-id="55951-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55951-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



