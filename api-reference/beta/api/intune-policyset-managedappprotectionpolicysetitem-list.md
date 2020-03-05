---
title: Список Манажедапппротектионполицисетитемс
description: Список свойств и связей объектов Манажедапппротектионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab945530251d00598d1a0a4c7920a82617f8a080
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460887"
---
# <a name="list-managedappprotectionpolicysetitems"></a><span data-ttu-id="752be-103">Список Манажедапппротектионполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="752be-103">List managedAppProtectionPolicySetItems</span></span>

<span data-ttu-id="752be-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="752be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="752be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="752be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="752be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="752be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="752be-107">Список свойств и связей объектов [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="752be-107">List properties and relationships of the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="752be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="752be-108">Prerequisites</span></span>
<span data-ttu-id="752be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="752be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="752be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="752be-111">Permission type</span></span>|<span data-ttu-id="752be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="752be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="752be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="752be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="752be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="752be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="752be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="752be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="752be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="752be-116">Not supported.</span></span>|
|<span data-ttu-id="752be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="752be-117">Application</span></span>|<span data-ttu-id="752be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="752be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="752be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="752be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="752be-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="752be-120">Request headers</span></span>
|<span data-ttu-id="752be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="752be-121">Header</span></span>|<span data-ttu-id="752be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="752be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="752be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="752be-123">Authorization</span></span>|<span data-ttu-id="752be-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="752be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="752be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="752be-125">Accept</span></span>|<span data-ttu-id="752be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="752be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="752be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="752be-127">Request body</span></span>
<span data-ttu-id="752be-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="752be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="752be-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="752be-129">Response</span></span>
<span data-ttu-id="752be-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="752be-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="752be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="752be-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="752be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="752be-132">Request</span></span>
<span data-ttu-id="752be-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="752be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="752be-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="752be-134">Response</span></span>
<span data-ttu-id="752be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="752be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 646

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
      "id": "e10d79c9-79c9-e10d-c979-0de1c9790de1",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "targetedAppManagementLevels": "Targeted App Management Levels value"
    }
  ]
}
```





