---
title: Получение androidWiFiConfiguration
description: Чтение свойства и связи объекта androidWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5a220c9b9235aa843819f57aacb8175b4df94004
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410590"
---
# <a name="get-androidwificonfiguration"></a><span data-ttu-id="64c42-103">Получение androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="64c42-103">Get androidWiFiConfiguration</span></span>

> <span data-ttu-id="64c42-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64c42-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64c42-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64c42-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64c42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64c42-107">Чтение свойства и связи объекта [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64c42-107">Read properties and relationships of the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64c42-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="64c42-108">Prerequisites</span></span>
<span data-ttu-id="64c42-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="64c42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64c42-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c42-111">Permission type</span></span>|<span data-ttu-id="64c42-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64c42-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64c42-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64c42-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64c42-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64c42-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c42-116">Not supported.</span></span>|
|<span data-ttu-id="64c42-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64c42-117">Application</span></span>|<span data-ttu-id="64c42-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64c42-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64c42-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64c42-120">Optional query parameters</span></span>
<span data-ttu-id="64c42-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64c42-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64c42-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64c42-122">Request headers</span></span>
|<span data-ttu-id="64c42-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64c42-123">Header</span></span>|<span data-ttu-id="64c42-124">Значение</span><span class="sxs-lookup"><span data-stu-id="64c42-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64c42-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="64c42-125">Authorization</span></span>|<span data-ttu-id="64c42-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="64c42-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64c42-127">Accept</span><span class="sxs-lookup"><span data-stu-id="64c42-127">Accept</span></span>|<span data-ttu-id="64c42-128">application/json</span><span class="sxs-lookup"><span data-stu-id="64c42-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64c42-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64c42-129">Request body</span></span>
<span data-ttu-id="64c42-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64c42-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64c42-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c42-131">Response</span></span>
<span data-ttu-id="64c42-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64c42-132">If successful, this method returns a `200 OK` response code and [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64c42-133">Пример</span><span class="sxs-lookup"><span data-stu-id="64c42-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="64c42-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c42-134">Request</span></span>
<span data-ttu-id="64c42-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64c42-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="64c42-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c42-136">Response</span></span>
<span data-ttu-id="64c42-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64c42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 658

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
    "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaEnterprise"
  }
}
```




