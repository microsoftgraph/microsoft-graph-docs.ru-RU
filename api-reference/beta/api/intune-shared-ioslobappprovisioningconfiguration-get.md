---
title: Get iosLobAppProvisioningConfiguration
description: Чтение свойств и связей объекта iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76646d93979c15604a9dce14a6e524903a958e80
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863165"
---
# <a name="get-ioslobappprovisioningconfiguration"></a><span data-ttu-id="94e9f-103">Get iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="94e9f-103">Get iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="94e9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94e9f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94e9f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94e9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94e9f-107">Чтение свойств и связей объекта [iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94e9f-107">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94e9f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="94e9f-108">Prerequisites</span></span>
<span data-ttu-id="94e9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e9f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94e9f-111">Permission type</span></span>|<span data-ttu-id="94e9f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94e9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94e9f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94e9f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="94e9f-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="94e9f-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="94e9f-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e9f-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="94e9f-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="94e9f-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="94e9f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e9f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="94e9f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94e9f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e9f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e9f-119">Not supported.</span></span>|
|<span data-ttu-id="94e9f-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="94e9f-120">Application</span></span>||
| <span data-ttu-id="94e9f-121">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="94e9f-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="94e9f-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e9f-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="94e9f-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="94e9f-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="94e9f-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e9f-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94e9f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94e9f-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94e9f-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94e9f-126">Optional query parameters</span></span>
<span data-ttu-id="94e9f-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94e9f-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94e9f-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94e9f-128">Request headers</span></span>
|<span data-ttu-id="94e9f-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94e9f-129">Header</span></span>|<span data-ttu-id="94e9f-130">Значение</span><span class="sxs-lookup"><span data-stu-id="94e9f-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94e9f-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94e9f-131">Authorization</span></span>|<span data-ttu-id="94e9f-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94e9f-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94e9f-133">Accept</span><span class="sxs-lookup"><span data-stu-id="94e9f-133">Accept</span></span>|<span data-ttu-id="94e9f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="94e9f-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e9f-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94e9f-135">Request body</span></span>
<span data-ttu-id="94e9f-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94e9f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e9f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="94e9f-137">Response</span></span>
<span data-ttu-id="94e9f-138">В случае успеха этот метод возвращает код отклика и `200 OK` [объект iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="94e9f-138">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e9f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="94e9f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="94e9f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="94e9f-140">Request</span></span>
<span data-ttu-id="94e9f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94e9f-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="94e9f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="94e9f-142">Response</span></span>
<span data-ttu-id="94e9f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94e9f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







