---
title: Список iosLobAppProvisioningConfigurations
description: Список свойств и связей объектов iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d1d8db1a0703fcf40148929e214ae7851facaa82
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729913"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="45516-103">Список iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="45516-103">List iosLobAppProvisioningConfigurations</span></span>

<span data-ttu-id="45516-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45516-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45516-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45516-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45516-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45516-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45516-107">Список свойств и связей объектов [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45516-107">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45516-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45516-108">Prerequisites</span></span>
<span data-ttu-id="45516-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45516-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45516-111">Permission type</span></span>|<span data-ttu-id="45516-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45516-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45516-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45516-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="45516-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="45516-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="45516-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45516-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="45516-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="45516-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="45516-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45516-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45516-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45516-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45516-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45516-119">Not supported.</span></span>|
|<span data-ttu-id="45516-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45516-120">Application</span></span>||
| <span data-ttu-id="45516-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="45516-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="45516-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45516-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="45516-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="45516-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="45516-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45516-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45516-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45516-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45516-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45516-126">Request headers</span></span>
|<span data-ttu-id="45516-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45516-127">Header</span></span>|<span data-ttu-id="45516-128">Значение</span><span class="sxs-lookup"><span data-stu-id="45516-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45516-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45516-129">Authorization</span></span>|<span data-ttu-id="45516-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45516-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45516-131">Accept</span><span class="sxs-lookup"><span data-stu-id="45516-131">Accept</span></span>|<span data-ttu-id="45516-132">application/json</span><span class="sxs-lookup"><span data-stu-id="45516-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45516-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45516-133">Request body</span></span>
<span data-ttu-id="45516-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45516-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45516-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="45516-135">Response</span></span>
<span data-ttu-id="45516-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45516-136">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45516-137">Пример</span><span class="sxs-lookup"><span data-stu-id="45516-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="45516-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="45516-138">Request</span></span>
<span data-ttu-id="45516-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45516-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="45516-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="45516-140">Response</span></span>
<span data-ttu-id="45516-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45516-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








