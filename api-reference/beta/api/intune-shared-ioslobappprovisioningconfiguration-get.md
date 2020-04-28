---
title: Получение iosLobAppProvisioningConfiguration
description: Чтение свойств и связей объекта iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c1e04875f68a16fd36ce5e89bd70622448331fa
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453847"
---
# <a name="get-ioslobappprovisioningconfiguration"></a><span data-ttu-id="d3a59-103">Получение iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3a59-103">Get iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="d3a59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3a59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3a59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3a59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a59-107">Чтение свойств и связей объекта [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d3a59-107">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3a59-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3a59-108">Prerequisites</span></span>
<span data-ttu-id="d3a59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3a59-111">Permission type</span></span>|<span data-ttu-id="d3a59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3a59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3a59-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d3a59-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="d3a59-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d3a59-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a59-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="d3a59-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d3a59-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d3a59-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a59-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3a59-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3a59-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a59-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a59-119">Not supported.</span></span>|
|<span data-ttu-id="d3a59-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3a59-120">Application</span></span>||
| <span data-ttu-id="d3a59-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="d3a59-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d3a59-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a59-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="d3a59-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d3a59-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d3a59-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a59-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a59-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3a59-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3a59-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3a59-126">Optional query parameters</span></span>
<span data-ttu-id="d3a59-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d3a59-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3a59-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3a59-128">Request headers</span></span>
|<span data-ttu-id="d3a59-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3a59-129">Header</span></span>|<span data-ttu-id="d3a59-130">Значение</span><span class="sxs-lookup"><span data-stu-id="d3a59-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3a59-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3a59-131">Authorization</span></span>|<span data-ttu-id="d3a59-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3a59-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3a59-133">Accept</span><span class="sxs-lookup"><span data-stu-id="d3a59-133">Accept</span></span>|<span data-ttu-id="d3a59-134">application/json</span><span class="sxs-lookup"><span data-stu-id="d3a59-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a59-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3a59-135">Request body</span></span>
<span data-ttu-id="d3a59-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3a59-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a59-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3a59-137">Response</span></span>
<span data-ttu-id="d3a59-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3a59-138">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a59-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d3a59-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3a59-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3a59-140">Request</span></span>
<span data-ttu-id="d3a59-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3a59-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d3a59-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3a59-142">Response</span></span>
<span data-ttu-id="d3a59-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3a59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": {
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
}
```






