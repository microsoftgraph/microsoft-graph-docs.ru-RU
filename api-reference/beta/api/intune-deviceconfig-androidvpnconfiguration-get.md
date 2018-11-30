---
title: Получение androidVpnConfiguration
description: Чтение свойства и связи объекта androidVpnConfiguration.
ms.openlocfilehash: e6f863a589f042cb27098ea8f82cf2c61a424b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076904"
---
# <a name="get-androidvpnconfiguration"></a><span data-ttu-id="3eb4f-103">Получение androidVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3eb4f-103">Get androidVpnConfiguration</span></span>

> <span data-ttu-id="3eb4f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eb4f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eb4f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3eb4f-107">Чтение свойства и связи объекта [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3eb4f-107">Read properties and relationships of the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3eb4f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3eb4f-108">Prerequisites</span></span>
<span data-ttu-id="3eb4f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eb4f-111">Permission type</span></span>|<span data-ttu-id="3eb4f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eb4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb4f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eb4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb4f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eb4f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3eb4f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eb4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-116">Not supported.</span></span>|
|<span data-ttu-id="3eb4f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3eb4f-117">Application</span></span>|<span data-ttu-id="3eb4f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eb4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3eb4f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3eb4f-120">Optional query parameters</span></span>
<span data-ttu-id="3eb4f-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3eb4f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3eb4f-122">Request headers</span></span>
|<span data-ttu-id="3eb4f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3eb4f-123">Header</span></span>|<span data-ttu-id="3eb4f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3eb4f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb4f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb4f-125">Authorization</span></span>|<span data-ttu-id="3eb4f-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3eb4f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb4f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3eb4f-127">Accept</span></span>|<span data-ttu-id="3eb4f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb4f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb4f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eb4f-129">Request body</span></span>
<span data-ttu-id="3eb4f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eb4f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3eb4f-131">Response</span></span>
<span data-ttu-id="3eb4f-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-132">If successful, this method returns a `200 OK` response code and [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb4f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3eb4f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3eb4f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eb4f-134">Request</span></span>
<span data-ttu-id="3eb4f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eb4f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3eb4f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="3eb4f-136">Response</span></span>
<span data-ttu-id="3eb4f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3eb4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "value": {
    "@odata.type": "#microsoft.graph.androidVpnConfiguration",
    "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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





