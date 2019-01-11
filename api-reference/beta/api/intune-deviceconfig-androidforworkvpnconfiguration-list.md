---
title: Список androidForWorkVpnConfigurations
description: Свойства списка и связей объектов androidForWorkVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 81816923c27d604b9002c49e88ed573a4e126713
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817502"
---
# <a name="list-androidforworkvpnconfigurations"></a><span data-ttu-id="0ca65-103">Список androidForWorkVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="0ca65-103">List androidForWorkVpnConfigurations</span></span>

> <span data-ttu-id="0ca65-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ca65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ca65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ca65-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ca65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ca65-107">Свойства списка и связей объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0ca65-107">List properties and relationships of the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ca65-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ca65-108">Prerequisites</span></span>
<span data-ttu-id="0ca65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ca65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ca65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ca65-111">Permission type</span></span>|<span data-ttu-id="0ca65-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ca65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ca65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ca65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ca65-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ca65-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ca65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ca65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ca65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca65-116">Not supported.</span></span>|
|<span data-ttu-id="0ca65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ca65-117">Application</span></span>|<span data-ttu-id="0ca65-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ca65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ca65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ca65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ca65-120">Request headers</span></span>
|<span data-ttu-id="0ca65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ca65-121">Header</span></span>|<span data-ttu-id="0ca65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ca65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ca65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ca65-123">Authorization</span></span>|<span data-ttu-id="0ca65-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ca65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ca65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ca65-125">Accept</span></span>|<span data-ttu-id="0ca65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ca65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ca65-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ca65-127">Request body</span></span>
<span data-ttu-id="0ca65-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ca65-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ca65-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ca65-129">Response</span></span>
<span data-ttu-id="0ca65-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ca65-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ca65-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ca65-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ca65-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ca65-132">Request</span></span>
<span data-ttu-id="0ca65-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ca65-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0ca65-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ca65-134">Response</span></span>
<span data-ttu-id="0ca65-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ca65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1346

{
  "value": [
    {
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
  ]
}
```





