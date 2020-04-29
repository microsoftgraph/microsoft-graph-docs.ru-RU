---
title: Get deviceConfiguration
description: Чтение свойств и связей объекта deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbdb958c7e92c24b4a393af008a3cac0fa00e3fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470426"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="e8589-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8589-103">Get deviceConfiguration</span></span>

<span data-ttu-id="e8589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8589-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8589-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8589-106">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8589-106">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8589-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e8589-107">Prerequisites</span></span>
<span data-ttu-id="e8589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8589-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8589-110">Permission type</span></span>|<span data-ttu-id="e8589-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8589-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8589-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8589-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8589-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8589-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e8589-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8589-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8589-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8589-115">Not supported.</span></span>|
|<span data-ttu-id="e8589-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8589-116">Application</span></span>|<span data-ttu-id="e8589-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8589-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8589-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8589-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8589-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8589-119">Optional query parameters</span></span>
<span data-ttu-id="e8589-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8589-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8589-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8589-121">Request headers</span></span>
|<span data-ttu-id="e8589-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8589-122">Header</span></span>|<span data-ttu-id="e8589-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e8589-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8589-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8589-124">Authorization</span></span>|<span data-ttu-id="e8589-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8589-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8589-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e8589-126">Accept</span></span>|<span data-ttu-id="e8589-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8589-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8589-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8589-128">Request body</span></span>
<span data-ttu-id="e8589-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8589-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8589-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8589-130">Response</span></span>
<span data-ttu-id="e8589-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8589-131">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8589-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e8589-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8589-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8589-133">Request</span></span>
<span data-ttu-id="e8589-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8589-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e8589-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8589-135">Response</span></span>
<span data-ttu-id="e8589-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8589-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "34977265-7265-3497-6572-973465729734",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```






