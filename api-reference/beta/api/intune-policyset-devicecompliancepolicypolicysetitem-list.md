---
title: Список Девицекомплианцеполициполицисетитемс
description: Список свойств и связей объектов Девицекомплианцеполициполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afbc50a3c904771796083632610fae2873b9c3b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726019"
---
# <a name="list-devicecompliancepolicypolicysetitems"></a><span data-ttu-id="6adf8-103">Список Девицекомплианцеполициполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="6adf8-103">List deviceCompliancePolicyPolicySetItems</span></span>

<span data-ttu-id="6adf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6adf8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6adf8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6adf8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6adf8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6adf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6adf8-107">Список свойств и связей объектов [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="6adf8-107">List properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6adf8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6adf8-108">Prerequisites</span></span>
<span data-ttu-id="6adf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6adf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6adf8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6adf8-111">Permission type</span></span>|<span data-ttu-id="6adf8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6adf8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6adf8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6adf8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6adf8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6adf8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6adf8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6adf8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6adf8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6adf8-116">Not supported.</span></span>|
|<span data-ttu-id="6adf8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6adf8-117">Application</span></span>|<span data-ttu-id="6adf8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6adf8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6adf8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6adf8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="6adf8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6adf8-120">Request headers</span></span>
|<span data-ttu-id="6adf8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6adf8-121">Header</span></span>|<span data-ttu-id="6adf8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6adf8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6adf8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6adf8-123">Authorization</span></span>|<span data-ttu-id="6adf8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6adf8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6adf8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6adf8-125">Accept</span></span>|<span data-ttu-id="6adf8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6adf8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6adf8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6adf8-127">Request body</span></span>
<span data-ttu-id="6adf8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6adf8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6adf8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6adf8-129">Response</span></span>
<span data-ttu-id="6adf8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6adf8-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6adf8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6adf8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6adf8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6adf8-132">Request</span></span>
<span data-ttu-id="6adf8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6adf8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="6adf8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6adf8-134">Response</span></span>
<span data-ttu-id="6adf8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6adf8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
      "id": "5c0bc827-c827-5c0b-27c8-0b5c27c80b5c",
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





