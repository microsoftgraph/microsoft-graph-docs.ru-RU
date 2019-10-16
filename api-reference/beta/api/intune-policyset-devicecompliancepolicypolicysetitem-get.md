---
title: Получение Девицекомплианцеполициполицисетитем
description: Чтение свойств и связей объекта Девицекомплианцеполициполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de2a895af3df0674e0193e1408abd5bbc54450b8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537617"
---
# <a name="get-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="778d9-103">Получение Девицекомплианцеполициполицисетитем</span><span class="sxs-lookup"><span data-stu-id="778d9-103">Get deviceCompliancePolicyPolicySetItem</span></span>

> <span data-ttu-id="778d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="778d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="778d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="778d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="778d9-106">Чтение свойств и связей объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="778d9-106">Read properties and relationships of the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="778d9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="778d9-107">Prerequisites</span></span>
<span data-ttu-id="778d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="778d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="778d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="778d9-110">Permission type</span></span>|<span data-ttu-id="778d9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="778d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="778d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="778d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="778d9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="778d9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="778d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="778d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="778d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="778d9-115">Not supported.</span></span>|
|<span data-ttu-id="778d9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="778d9-116">Application</span></span>|<span data-ttu-id="778d9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="778d9-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="778d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="778d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="778d9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="778d9-119">Optional query parameters</span></span>
<span data-ttu-id="778d9-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="778d9-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="778d9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="778d9-121">Request headers</span></span>
|<span data-ttu-id="778d9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="778d9-122">Header</span></span>|<span data-ttu-id="778d9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="778d9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="778d9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="778d9-124">Authorization</span></span>|<span data-ttu-id="778d9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="778d9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="778d9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="778d9-126">Accept</span></span>|<span data-ttu-id="778d9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="778d9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="778d9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="778d9-128">Request body</span></span>
<span data-ttu-id="778d9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="778d9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="778d9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="778d9-130">Response</span></span>
<span data-ttu-id="778d9-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="778d9-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="778d9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="778d9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="778d9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="778d9-133">Request</span></span>
<span data-ttu-id="778d9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="778d9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="778d9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="778d9-135">Response</span></span>
<span data-ttu-id="778d9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="778d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
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
}
```






