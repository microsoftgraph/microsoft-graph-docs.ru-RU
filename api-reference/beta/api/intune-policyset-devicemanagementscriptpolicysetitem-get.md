---
title: Получение Девицеманажементскриптполицисетитем
description: Чтение свойств и связей объекта Девицеманажементскриптполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e0826060b99f894b33807772db150c990f09f26
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224195"
---
# <a name="get-devicemanagementscriptpolicysetitem"></a><span data-ttu-id="8e170-103">Получение Девицеманажементскриптполицисетитем</span><span class="sxs-lookup"><span data-stu-id="8e170-103">Get deviceManagementScriptPolicySetItem</span></span>

<span data-ttu-id="8e170-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e170-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e170-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e170-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e170-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e170-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e170-107">Чтение свойств и связей объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="8e170-107">Read properties and relationships of the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e170-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e170-108">Prerequisites</span></span>
<span data-ttu-id="8e170-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e170-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e170-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e170-111">Permission type</span></span>|<span data-ttu-id="8e170-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e170-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e170-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e170-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e170-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e170-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8e170-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e170-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e170-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e170-116">Not supported.</span></span>|
|<span data-ttu-id="8e170-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e170-117">Application</span></span>|<span data-ttu-id="8e170-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e170-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e170-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e170-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e170-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e170-120">Optional query parameters</span></span>
<span data-ttu-id="8e170-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e170-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e170-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e170-122">Request headers</span></span>
|<span data-ttu-id="8e170-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e170-123">Header</span></span>|<span data-ttu-id="8e170-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8e170-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e170-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e170-125">Authorization</span></span>|<span data-ttu-id="8e170-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e170-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e170-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8e170-127">Accept</span></span>|<span data-ttu-id="8e170-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8e170-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e170-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e170-129">Request body</span></span>
<span data-ttu-id="8e170-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e170-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e170-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e170-131">Response</span></span>
<span data-ttu-id="8e170-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e170-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e170-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8e170-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e170-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e170-134">Request</span></span>
<span data-ttu-id="8e170-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e170-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="8e170-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e170-136">Response</span></span>
<span data-ttu-id="8e170-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e170-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




