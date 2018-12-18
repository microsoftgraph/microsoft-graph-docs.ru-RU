---
title: Получение unsupportedDeviceConfiguration
description: Чтение свойства и связи объекта unsupportedDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 9b6b350356d59b3792ca533c3fa65053e7113fa7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355939"
---
# <a name="get-unsupporteddeviceconfiguration"></a><span data-ttu-id="8dade-103">Получение unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dade-103">Get unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="8dade-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8dade-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dade-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dade-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8dade-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8dade-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dade-107">Чтение свойства и связи объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8dade-107">Read properties and relationships of the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8dade-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8dade-108">Prerequisites</span></span>
<span data-ttu-id="8dade-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dade-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dade-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dade-111">Permission type</span></span>|<span data-ttu-id="8dade-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dade-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dade-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dade-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dade-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dade-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8dade-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dade-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dade-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dade-116">Not supported.</span></span>|
|<span data-ttu-id="8dade-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dade-117">Application</span></span>|<span data-ttu-id="8dade-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dade-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dade-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dade-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8dade-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8dade-120">Optional query parameters</span></span>
<span data-ttu-id="8dade-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8dade-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8dade-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dade-122">Request headers</span></span>
|<span data-ttu-id="8dade-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dade-123">Header</span></span>|<span data-ttu-id="8dade-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8dade-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dade-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dade-125">Authorization</span></span>|<span data-ttu-id="8dade-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8dade-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dade-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8dade-127">Accept</span></span>|<span data-ttu-id="8dade-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8dade-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dade-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dade-129">Request body</span></span>
<span data-ttu-id="8dade-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8dade-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dade-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8dade-131">Response</span></span>
<span data-ttu-id="8dade-132">Успешно завершена, этот метод возвращает `200 OK` объект [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8dade-132">If successful, this method returns a `200 OK` response code and [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dade-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8dade-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8dade-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dade-134">Request</span></span>
<span data-ttu-id="8dade-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dade-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8dade-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8dade-136">Response</span></span>
<span data-ttu-id="8dade-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8dade-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





