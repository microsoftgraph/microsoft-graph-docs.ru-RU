---
title: Список androidForWorkVpnConfigurations
description: Свойства списка и связей объектов androidForWorkVpnConfiguration.
author: tfitzmac
ms.openlocfilehash: ca56e8033563166f80aa5e364f716b9bc4c38c0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344725"
---
# <a name="list-androidforworkvpnconfigurations"></a><span data-ttu-id="962bf-103">Список androidForWorkVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="962bf-103">List androidForWorkVpnConfigurations</span></span>

> <span data-ttu-id="962bf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="962bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="962bf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="962bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="962bf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="962bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="962bf-107">Свойства списка и связей объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="962bf-107">List properties and relationships of the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="962bf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="962bf-108">Prerequisites</span></span>
<span data-ttu-id="962bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="962bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="962bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="962bf-111">Permission type</span></span>|<span data-ttu-id="962bf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="962bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="962bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="962bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="962bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="962bf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="962bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="962bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="962bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="962bf-116">Not supported.</span></span>|
|<span data-ttu-id="962bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="962bf-117">Application</span></span>|<span data-ttu-id="962bf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="962bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="962bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="962bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="962bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="962bf-120">Request headers</span></span>
|<span data-ttu-id="962bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="962bf-121">Header</span></span>|<span data-ttu-id="962bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="962bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="962bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="962bf-123">Authorization</span></span>|<span data-ttu-id="962bf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="962bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="962bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="962bf-125">Accept</span></span>|<span data-ttu-id="962bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="962bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="962bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="962bf-127">Request body</span></span>
<span data-ttu-id="962bf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="962bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="962bf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="962bf-129">Response</span></span>
<span data-ttu-id="962bf-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="962bf-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="962bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="962bf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="962bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="962bf-132">Request</span></span>
<span data-ttu-id="962bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="962bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="962bf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="962bf-134">Response</span></span>
<span data-ttu-id="962bf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="962bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





