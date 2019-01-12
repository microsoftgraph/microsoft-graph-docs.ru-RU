---
title: Список macOSEndpointProtectionConfigurations
description: Свойства списка и связей объектов macOSEndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b9e71b18c037f6e8daff10f65cb500df4e0424b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978440"
---
# <a name="list-macosendpointprotectionconfigurations"></a><span data-ttu-id="90902-103">Список macOSEndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="90902-103">List macOSEndpointProtectionConfigurations</span></span>

> <span data-ttu-id="90902-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90902-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90902-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90902-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90902-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="90902-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90902-107">Свойства списка и связей объектов [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="90902-107">List properties and relationships of the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90902-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90902-108">Prerequisites</span></span>
<span data-ttu-id="90902-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90902-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90902-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90902-111">Permission type</span></span>|<span data-ttu-id="90902-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90902-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90902-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90902-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90902-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90902-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90902-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90902-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90902-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90902-116">Not supported.</span></span>|
|<span data-ttu-id="90902-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90902-117">Application</span></span>|<span data-ttu-id="90902-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90902-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90902-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90902-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90902-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90902-120">Request headers</span></span>
|<span data-ttu-id="90902-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90902-121">Header</span></span>|<span data-ttu-id="90902-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90902-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90902-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90902-123">Authorization</span></span>|<span data-ttu-id="90902-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="90902-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90902-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90902-125">Accept</span></span>|<span data-ttu-id="90902-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90902-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90902-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90902-127">Request body</span></span>
<span data-ttu-id="90902-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90902-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90902-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="90902-129">Response</span></span>
<span data-ttu-id="90902-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="90902-130">If successful, this method returns a `200 OK` response code and a collection of [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90902-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90902-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="90902-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90902-132">Request</span></span>
<span data-ttu-id="90902-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90902-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="90902-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="90902-134">Response</span></span>
<span data-ttu-id="90902-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="90902-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 944

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
      "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "gatekeeperAllowedAppSource": "macAppStore",
      "gatekeeperBlockOverride": true,
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true,
      "firewallApplications": [
        {
          "@odata.type": "microsoft.graph.macOSFirewallApplication",
          "bundleId": "Bundle Id value",
          "allowsIncomingConnections": true
        }
      ]
    }
  ]
}
```





