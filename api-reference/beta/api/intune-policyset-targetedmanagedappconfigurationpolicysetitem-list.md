---
title: Список Таржетедманажедаппконфигуратионполицисетитемс
description: Список свойств и связей объектов Таржетедманажедаппконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e96da6c7c808c5dc7c077a79a8cd888e17c79aed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375147"
---
# <a name="list-targetedmanagedappconfigurationpolicysetitems"></a><span data-ttu-id="f8e96-103">Список Таржетедманажедаппконфигуратионполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="f8e96-103">List targetedManagedAppConfigurationPolicySetItems</span></span>

<span data-ttu-id="f8e96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8e96-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8e96-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8e96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e96-107">Список свойств и связей объектов [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="f8e96-107">List properties and relationships of the [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8e96-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8e96-108">Prerequisites</span></span>
<span data-ttu-id="f8e96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8e96-111">Permission type</span></span>|<span data-ttu-id="f8e96-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8e96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8e96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8e96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8e96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f8e96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8e96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8e96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e96-116">Not supported.</span></span>|
|<span data-ttu-id="f8e96-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f8e96-117">Application</span></span>|<span data-ttu-id="f8e96-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e96-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8e96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8e96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="f8e96-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8e96-120">Request headers</span></span>
|<span data-ttu-id="f8e96-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8e96-121">Header</span></span>|<span data-ttu-id="f8e96-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8e96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8e96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8e96-123">Authorization</span></span>|<span data-ttu-id="f8e96-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8e96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8e96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8e96-125">Accept</span></span>|<span data-ttu-id="f8e96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8e96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8e96-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8e96-127">Request body</span></span>
<span data-ttu-id="f8e96-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8e96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8e96-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8e96-129">Response</span></span>
<span data-ttu-id="f8e96-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8e96-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e96-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8e96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8e96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8e96-132">Request</span></span>
<span data-ttu-id="f8e96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8e96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="f8e96-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8e96-134">Response</span></span>
<span data-ttu-id="f8e96-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8e96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 579

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
      "id": "f86d3112-3112-f86d-1231-6df812316df8",
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



