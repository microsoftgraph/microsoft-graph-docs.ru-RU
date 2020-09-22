---
title: Список Иослобапппровисионингконфигуратионполицисетитемс
description: Список свойств и связей объектов Иослобапппровисионингконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba936fede91cd2a2a010847afd78aedc65e93c9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093478"
---
# <a name="list-ioslobappprovisioningconfigurationpolicysetitems"></a><span data-ttu-id="ea150-103">Список Иослобапппровисионингконфигуратионполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="ea150-103">List iosLobAppProvisioningConfigurationPolicySetItems</span></span>

<span data-ttu-id="ea150-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea150-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea150-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea150-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea150-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea150-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea150-107">Список свойств и связей объектов [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ea150-107">List properties and relationships of the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea150-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea150-108">Prerequisites</span></span>
<span data-ttu-id="ea150-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea150-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea150-111">Permission type</span></span>|<span data-ttu-id="ea150-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea150-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea150-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea150-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea150-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea150-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea150-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea150-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea150-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea150-116">Not supported.</span></span>|
|<span data-ttu-id="ea150-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea150-117">Application</span></span>|<span data-ttu-id="ea150-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea150-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea150-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea150-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="ea150-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea150-120">Request headers</span></span>
|<span data-ttu-id="ea150-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea150-121">Header</span></span>|<span data-ttu-id="ea150-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea150-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea150-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea150-123">Authorization</span></span>|<span data-ttu-id="ea150-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea150-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea150-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea150-125">Accept</span></span>|<span data-ttu-id="ea150-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea150-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea150-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea150-127">Request body</span></span>
<span data-ttu-id="ea150-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea150-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea150-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea150-129">Response</span></span>
<span data-ttu-id="ea150-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea150-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea150-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ea150-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea150-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea150-132">Request</span></span>
<span data-ttu-id="ea150-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea150-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="ea150-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea150-134">Response</span></span>
<span data-ttu-id="ea150-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea150-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
      "id": "6a978d58-8d58-6a97-588d-976a588d976a",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```






