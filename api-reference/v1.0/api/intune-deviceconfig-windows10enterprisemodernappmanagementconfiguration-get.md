---
title: Get windows10EnterpriseModernAppManagementConfiguration
description: Чтение свойств и связей объекта windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f9661101616bd26478de0fec5c76178d84c1318
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930021"
---
# <a name="get-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="b2dd8-103">Get windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2dd8-103">Get windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="b2dd8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2dd8-105">Чтение свойств и связей объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2dd8-105">Read properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2dd8-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b2dd8-106">Prerequisites</span></span>
<span data-ttu-id="b2dd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2dd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2dd8-109">Permission type</span></span>|<span data-ttu-id="b2dd8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2dd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2dd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2dd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2dd8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2dd8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2dd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2dd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2dd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-114">Not supported.</span></span>|
|<span data-ttu-id="b2dd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2dd8-115">Application</span></span>|<span data-ttu-id="b2dd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2dd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2dd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2dd8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2dd8-118">Optional query parameters</span></span>
<span data-ttu-id="b2dd8-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b2dd8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2dd8-120">Request headers</span></span>
|<span data-ttu-id="b2dd8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2dd8-121">Header</span></span>|<span data-ttu-id="b2dd8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2dd8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2dd8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2dd8-123">Authorization</span></span>|<span data-ttu-id="b2dd8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2dd8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2dd8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2dd8-125">Accept</span></span>|<span data-ttu-id="b2dd8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2dd8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2dd8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2dd8-127">Request body</span></span>
<span data-ttu-id="b2dd8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2dd8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2dd8-129">Response</span></span>
<span data-ttu-id="b2dd8-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-130">If successful, this method returns a `200 OK` response code and [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2dd8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b2dd8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2dd8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2dd8-132">Request</span></span>
<span data-ttu-id="b2dd8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b2dd8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2dd8-134">Response</span></span>
<span data-ttu-id="b2dd8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2dd8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
    "id": "d6577687-7687-d657-8776-57d6877657d6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "uninstallBuiltInApps": true
  }
}
```



