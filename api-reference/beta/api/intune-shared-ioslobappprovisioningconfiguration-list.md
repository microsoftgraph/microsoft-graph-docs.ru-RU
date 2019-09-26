---
title: Список iosLobAppProvisioningConfigurations
description: Список свойств и связей объектов iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1da40eeacecd81ef9c95d18aa66f716745e3325
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201030"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="cfc69-103">Список iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="cfc69-103">List iosLobAppProvisioningConfigurations</span></span>

> <span data-ttu-id="cfc69-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfc69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfc69-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfc69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfc69-106">Список свойств и связей объектов [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cfc69-106">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfc69-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cfc69-107">Prerequisites</span></span>
<span data-ttu-id="cfc69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfc69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfc69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfc69-110">Permission type</span></span>|<span data-ttu-id="cfc69-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfc69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfc69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfc69-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cfc69-113">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="cfc69-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="cfc69-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfc69-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="cfc69-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="cfc69-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cfc69-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfc69-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cfc69-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfc69-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfc69-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfc69-118">Not supported.</span></span>|
|<span data-ttu-id="cfc69-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfc69-119">Application</span></span>||
| <span data-ttu-id="cfc69-120">&nbsp;&nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="cfc69-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="cfc69-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfc69-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="cfc69-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="cfc69-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cfc69-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfc69-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfc69-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfc69-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cfc69-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfc69-125">Request headers</span></span>
|<span data-ttu-id="cfc69-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cfc69-126">Header</span></span>|<span data-ttu-id="cfc69-127">Значение</span><span class="sxs-lookup"><span data-stu-id="cfc69-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfc69-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfc69-128">Authorization</span></span>|<span data-ttu-id="cfc69-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfc69-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfc69-130">Accept</span><span class="sxs-lookup"><span data-stu-id="cfc69-130">Accept</span></span>|<span data-ttu-id="cfc69-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cfc69-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfc69-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cfc69-132">Request body</span></span>
<span data-ttu-id="cfc69-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfc69-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfc69-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfc69-134">Response</span></span>
<span data-ttu-id="cfc69-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfc69-135">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfc69-136">Пример</span><span class="sxs-lookup"><span data-stu-id="cfc69-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfc69-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfc69-137">Request</span></span>
<span data-ttu-id="cfc69-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfc69-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="cfc69-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfc69-139">Response</span></span>
<span data-ttu-id="cfc69-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cfc69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
      "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA==",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




