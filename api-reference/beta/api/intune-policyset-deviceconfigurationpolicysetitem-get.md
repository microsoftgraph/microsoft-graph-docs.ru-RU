---
title: Получение Девицеконфигуратионполицисетитем
description: Чтение свойств и связей объекта Девицеконфигуратионполицисетитем.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: affa69563df9f5b84c48497c0c32aefdeff53097
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802414"
---
# <a name="get-deviceconfigurationpolicysetitem"></a><span data-ttu-id="53bb2-103">Получение Девицеконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="53bb2-103">Get deviceConfigurationPolicySetItem</span></span>

> <span data-ttu-id="53bb2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53bb2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53bb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53bb2-106">Чтение свойств и связей объекта [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="53bb2-106">Read properties and relationships of the [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53bb2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53bb2-107">Prerequisites</span></span>
<span data-ttu-id="53bb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53bb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53bb2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53bb2-110">Permission type</span></span>|<span data-ttu-id="53bb2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53bb2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53bb2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53bb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53bb2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="53bb2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="53bb2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53bb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53bb2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bb2-115">Not supported.</span></span>|
|<span data-ttu-id="53bb2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="53bb2-116">Application</span></span>|<span data-ttu-id="53bb2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="53bb2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53bb2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53bb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53bb2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53bb2-119">Optional query parameters</span></span>
<span data-ttu-id="53bb2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53bb2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53bb2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53bb2-121">Request headers</span></span>
|<span data-ttu-id="53bb2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53bb2-122">Header</span></span>|<span data-ttu-id="53bb2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="53bb2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53bb2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="53bb2-124">Authorization</span></span>|<span data-ttu-id="53bb2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53bb2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53bb2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="53bb2-126">Accept</span></span>|<span data-ttu-id="53bb2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="53bb2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53bb2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53bb2-128">Request body</span></span>
<span data-ttu-id="53bb2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53bb2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53bb2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="53bb2-130">Response</span></span>
<span data-ttu-id="53bb2-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53bb2-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53bb2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="53bb2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="53bb2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="53bb2-133">Request</span></span>
<span data-ttu-id="53bb2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53bb2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="53bb2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="53bb2-135">Response</span></span>
<span data-ttu-id="53bb2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53bb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
    "id": "00b1197c-197c-00b1-7c19-b1007c19b100",
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




