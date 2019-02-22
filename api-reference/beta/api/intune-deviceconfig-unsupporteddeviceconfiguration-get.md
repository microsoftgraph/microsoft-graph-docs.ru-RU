---
title: Получение Унсуппортеддевицеконфигуратион
description: Чтение свойств и связей объекта Унсуппортеддевицеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51ee16981e9a0eff07e93f2cb917a5ed174d5c2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162764"
---
# <a name="get-unsupporteddeviceconfiguration"></a><span data-ttu-id="5cd38-103">Получение Унсуппортеддевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5cd38-103">Get unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="5cd38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cd38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd38-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cd38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd38-106">Чтение свойств и связей объекта [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5cd38-106">Read properties and relationships of the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd38-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5cd38-107">Prerequisites</span></span>
<span data-ttu-id="5cd38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cd38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cd38-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cd38-110">Permission type</span></span>|<span data-ttu-id="5cd38-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cd38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd38-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cd38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd38-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cd38-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5cd38-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cd38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd38-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cd38-115">Not supported.</span></span>|
|<span data-ttu-id="5cd38-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cd38-116">Application</span></span>|<span data-ttu-id="5cd38-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cd38-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd38-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cd38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cd38-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cd38-119">Optional query parameters</span></span>
<span data-ttu-id="5cd38-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5cd38-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cd38-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cd38-121">Request headers</span></span>
|<span data-ttu-id="5cd38-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cd38-122">Header</span></span>|<span data-ttu-id="5cd38-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5cd38-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd38-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cd38-124">Authorization</span></span>|<span data-ttu-id="5cd38-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5cd38-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd38-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5cd38-126">Accept</span></span>|<span data-ttu-id="5cd38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd38-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd38-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cd38-128">Request body</span></span>
<span data-ttu-id="5cd38-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cd38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cd38-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cd38-130">Response</span></span>
<span data-ttu-id="5cd38-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cd38-131">If successful, this method returns a `200 OK` response code and [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd38-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5cd38-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd38-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cd38-133">Request</span></span>
<span data-ttu-id="5cd38-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cd38-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5cd38-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cd38-135">Response</span></span>
<span data-ttu-id="5cd38-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cd38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 747

{
  "value": {
    "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
    "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "originalEntityTypeName": "Original Entity Type Name value",
    "details": [
      {
        "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
        "message": "Message value",
        "propertyName": "Property Name value"
      }
    ]
  }
}
```




