---
title: Получение Таржетедманажедаппконфигуратионполицисетитем
description: Чтение свойств и связей объекта Таржетедманажедаппконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8996ae271fc4993db2ed8af82a350a5273b78b4e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940877"
---
# <a name="get-targetedmanagedappconfigurationpolicysetitem"></a><span data-ttu-id="463b7-103">Получение Таржетедманажедаппконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="463b7-103">Get targetedManagedAppConfigurationPolicySetItem</span></span>

> <span data-ttu-id="463b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="463b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="463b7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="463b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="463b7-106">Чтение свойств и связей объекта [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="463b7-106">Read properties and relationships of the [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="463b7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="463b7-107">Prerequisites</span></span>
<span data-ttu-id="463b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="463b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="463b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="463b7-110">Permission type</span></span>|<span data-ttu-id="463b7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="463b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="463b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="463b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="463b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="463b7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="463b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="463b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="463b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="463b7-115">Not supported.</span></span>|
|<span data-ttu-id="463b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="463b7-116">Application</span></span>|<span data-ttu-id="463b7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="463b7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="463b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="463b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="463b7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="463b7-119">Optional query parameters</span></span>
<span data-ttu-id="463b7-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="463b7-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="463b7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="463b7-121">Request headers</span></span>
|<span data-ttu-id="463b7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="463b7-122">Header</span></span>|<span data-ttu-id="463b7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="463b7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="463b7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="463b7-124">Authorization</span></span>|<span data-ttu-id="463b7-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="463b7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="463b7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="463b7-126">Accept</span></span>|<span data-ttu-id="463b7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="463b7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="463b7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="463b7-128">Request body</span></span>
<span data-ttu-id="463b7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="463b7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="463b7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="463b7-130">Response</span></span>
<span data-ttu-id="463b7-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [таржетедманажедаппконфигуратионполицисетитем](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="463b7-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="463b7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="463b7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="463b7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="463b7-133">Request</span></span>
<span data-ttu-id="463b7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="463b7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="463b7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="463b7-135">Response</span></span>
<span data-ttu-id="463b7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="463b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "value": {
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
}
```





