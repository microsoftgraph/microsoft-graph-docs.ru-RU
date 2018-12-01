---
title: Получение androidForWorkVpnConfiguration
description: Чтение свойства и связи объекта androidForWorkVpnConfiguration.
ms.openlocfilehash: 95da6115f0eb521f398aae3760e9895e95b59b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079291"
---
# <a name="get-androidforworkvpnconfiguration"></a><span data-ttu-id="47643-103">Получение androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="47643-103">Get androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="47643-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47643-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47643-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47643-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47643-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47643-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47643-107">Чтение свойства и связи объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="47643-107">Read properties and relationships of the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47643-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47643-108">Prerequisites</span></span>
<span data-ttu-id="47643-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47643-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47643-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47643-111">Permission type</span></span>|<span data-ttu-id="47643-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47643-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47643-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47643-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47643-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47643-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47643-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47643-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47643-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47643-116">Not supported.</span></span>|
|<span data-ttu-id="47643-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47643-117">Application</span></span>|<span data-ttu-id="47643-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47643-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47643-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47643-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47643-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47643-120">Optional query parameters</span></span>
<span data-ttu-id="47643-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47643-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="47643-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47643-122">Request headers</span></span>
|<span data-ttu-id="47643-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47643-123">Header</span></span>|<span data-ttu-id="47643-124">Значение</span><span class="sxs-lookup"><span data-stu-id="47643-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47643-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="47643-125">Authorization</span></span>|<span data-ttu-id="47643-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47643-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47643-127">Accept</span><span class="sxs-lookup"><span data-stu-id="47643-127">Accept</span></span>|<span data-ttu-id="47643-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47643-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47643-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47643-129">Request body</span></span>
<span data-ttu-id="47643-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47643-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47643-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="47643-131">Response</span></span>
<span data-ttu-id="47643-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47643-132">If successful, this method returns a `200 OK` response code and [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47643-133">Пример</span><span class="sxs-lookup"><span data-stu-id="47643-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="47643-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="47643-134">Request</span></span>
<span data-ttu-id="47643-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47643-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="47643-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="47643-136">Response</span></span>
<span data-ttu-id="47643-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="47643-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1254

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
    "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "connectionName": "Connection Name value",
    "connectionType": "pulseSecure",
    "role": "Role value",
    "realm": "Realm value",
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "fingerprint": "Fingerprint value",
    "customData": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ],
    "customKeyValueData": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "authenticationMethod": "usernameAndPassword"
  }
}
```





