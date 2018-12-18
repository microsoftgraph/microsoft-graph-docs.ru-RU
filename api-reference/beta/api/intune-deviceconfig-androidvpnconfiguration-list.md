---
title: Список androidVpnConfigurations
description: Свойства списка и связей объектов androidVpnConfiguration.
author: tfitzmac
ms.openlocfilehash: a26fe24e4680153075a54614b241ce7103d3caf2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354833"
---
# <a name="list-androidvpnconfigurations"></a><span data-ttu-id="4c250-103">Список androidVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="4c250-103">List androidVpnConfigurations</span></span>

> <span data-ttu-id="4c250-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c250-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c250-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c250-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c250-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c250-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c250-107">Свойства списка и связей объектов [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4c250-107">List properties and relationships of the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c250-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c250-108">Prerequisites</span></span>
<span data-ttu-id="4c250-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c250-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c250-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c250-111">Permission type</span></span>|<span data-ttu-id="4c250-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c250-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c250-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c250-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c250-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c250-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4c250-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c250-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c250-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c250-116">Not supported.</span></span>|
|<span data-ttu-id="4c250-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c250-117">Application</span></span>|<span data-ttu-id="4c250-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c250-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c250-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c250-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c250-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c250-120">Request headers</span></span>
|<span data-ttu-id="4c250-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c250-121">Header</span></span>|<span data-ttu-id="4c250-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c250-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c250-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c250-123">Authorization</span></span>|<span data-ttu-id="4c250-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c250-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c250-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c250-125">Accept</span></span>|<span data-ttu-id="4c250-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c250-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c250-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c250-127">Request body</span></span>
<span data-ttu-id="4c250-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c250-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c250-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c250-129">Response</span></span>
<span data-ttu-id="4c250-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4c250-130">If successful, this method returns a `200 OK` response code and a collection of [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c250-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4c250-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c250-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c250-132">Request</span></span>
<span data-ttu-id="4c250-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c250-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4c250-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c250-134">Response</span></span>
<span data-ttu-id="4c250-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c250-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "value": [
    {
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
  ]
}
```





