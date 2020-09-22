---
title: Получение Девицеманажементскриптполицисетитем
description: Чтение свойств и связей объекта Девицеманажементскриптполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3bce507ce9a970075fc12c16882565c778150fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093646"
---
# <a name="get-devicemanagementscriptpolicysetitem"></a><span data-ttu-id="b8213-103">Получение Девицеманажементскриптполицисетитем</span><span class="sxs-lookup"><span data-stu-id="b8213-103">Get deviceManagementScriptPolicySetItem</span></span>

<span data-ttu-id="b8213-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8213-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8213-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8213-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8213-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8213-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8213-107">Чтение свойств и связей объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b8213-107">Read properties and relationships of the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8213-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8213-108">Prerequisites</span></span>
<span data-ttu-id="b8213-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8213-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8213-111">Permission type</span></span>|<span data-ttu-id="b8213-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8213-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8213-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8213-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8213-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8213-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b8213-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8213-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8213-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8213-116">Not supported.</span></span>|
|<span data-ttu-id="b8213-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8213-117">Application</span></span>|<span data-ttu-id="b8213-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8213-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8213-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8213-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8213-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8213-120">Optional query parameters</span></span>
<span data-ttu-id="b8213-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b8213-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8213-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8213-122">Request headers</span></span>
|<span data-ttu-id="b8213-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8213-123">Header</span></span>|<span data-ttu-id="b8213-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b8213-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8213-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8213-125">Authorization</span></span>|<span data-ttu-id="b8213-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8213-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8213-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b8213-127">Accept</span></span>|<span data-ttu-id="b8213-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b8213-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8213-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8213-129">Request body</span></span>
<span data-ttu-id="b8213-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8213-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8213-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8213-131">Response</span></span>
<span data-ttu-id="b8213-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8213-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8213-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b8213-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8213-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8213-134">Request</span></span>
<span data-ttu-id="b8213-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8213-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="b8213-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8213-136">Response</span></span>
<span data-ttu-id="b8213-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8213-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
    "id": "b6b82c18-2c18-b6b8-182c-b8b6182cb8b6",
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






