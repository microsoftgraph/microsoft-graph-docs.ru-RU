---
title: Список Манажеддевицемобилеаппконфигуратионполицисетитемс
description: Список свойств и связей объектов Манажеддевицемобилеаппконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16a84b520388e5c1ac26fadb7b9f300822e4ce6a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460831"
---
# <a name="list-manageddevicemobileappconfigurationpolicysetitems"></a><span data-ttu-id="11950-103">Список Манажеддевицемобилеаппконфигуратионполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="11950-103">List managedDeviceMobileAppConfigurationPolicySetItems</span></span>

<span data-ttu-id="11950-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11950-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11950-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11950-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11950-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11950-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11950-107">Список свойств и связей объектов [манажеддевицемобилеаппконфигуратионполицисетитем](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="11950-107">List properties and relationships of the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11950-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="11950-108">Prerequisites</span></span>
<span data-ttu-id="11950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11950-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11950-111">Permission type</span></span>|<span data-ttu-id="11950-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11950-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11950-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11950-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11950-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="11950-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="11950-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11950-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11950-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11950-116">Not supported.</span></span>|
|<span data-ttu-id="11950-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11950-117">Application</span></span>|<span data-ttu-id="11950-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="11950-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11950-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11950-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="11950-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="11950-120">Request headers</span></span>
|<span data-ttu-id="11950-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11950-121">Header</span></span>|<span data-ttu-id="11950-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11950-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11950-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11950-123">Authorization</span></span>|<span data-ttu-id="11950-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11950-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11950-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11950-125">Accept</span></span>|<span data-ttu-id="11950-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11950-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11950-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11950-127">Request body</span></span>
<span data-ttu-id="11950-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11950-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11950-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="11950-129">Response</span></span>
<span data-ttu-id="11950-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажеддевицемобилеаппконфигуратионполицисетитем](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11950-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11950-131">Пример</span><span class="sxs-lookup"><span data-stu-id="11950-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="11950-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="11950-132">Request</span></span>
<span data-ttu-id="11950-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11950-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="11950-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="11950-134">Response</span></span>
<span data-ttu-id="11950-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11950-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 583

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
      "id": "bb065442-5442-bb06-4254-06bb425406bb",
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





