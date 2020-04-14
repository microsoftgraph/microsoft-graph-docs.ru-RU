---
title: Получение Енроллментрестриктионсконфигуратионполицисетитем
description: Чтение свойств и связей объекта Енроллментрестриктионсконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94567420873312b26a54899ae19b14ca82a4eeee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424155"
---
# <a name="get-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="dd3ee-103">Получение Енроллментрестриктионсконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="dd3ee-103">Get enrollmentRestrictionsConfigurationPolicySetItem</span></span>

<span data-ttu-id="dd3ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd3ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd3ee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd3ee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd3ee-107">Чтение свойств и связей объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="dd3ee-107">Read properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd3ee-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd3ee-108">Prerequisites</span></span>
<span data-ttu-id="dd3ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd3ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd3ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd3ee-111">Permission type</span></span>|<span data-ttu-id="dd3ee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd3ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd3ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd3ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd3ee-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd3ee-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dd3ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd3ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd3ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-116">Not supported.</span></span>|
|<span data-ttu-id="dd3ee-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd3ee-117">Application</span></span>|<span data-ttu-id="dd3ee-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd3ee-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd3ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd3ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd3ee-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd3ee-120">Optional query parameters</span></span>
<span data-ttu-id="dd3ee-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd3ee-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd3ee-122">Request headers</span></span>
|<span data-ttu-id="dd3ee-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd3ee-123">Header</span></span>|<span data-ttu-id="dd3ee-124">Значение</span><span class="sxs-lookup"><span data-stu-id="dd3ee-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd3ee-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd3ee-125">Authorization</span></span>|<span data-ttu-id="dd3ee-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd3ee-127">Accept</span><span class="sxs-lookup"><span data-stu-id="dd3ee-127">Accept</span></span>|<span data-ttu-id="dd3ee-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dd3ee-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd3ee-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd3ee-129">Request body</span></span>
<span data-ttu-id="dd3ee-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd3ee-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd3ee-131">Response</span></span>
<span data-ttu-id="dd3ee-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-132">If successful, this method returns a `200 OK` response code and [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd3ee-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dd3ee-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd3ee-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd3ee-134">Request</span></span>
<span data-ttu-id="dd3ee-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="dd3ee-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd3ee-136">Response</span></span>
<span data-ttu-id="dd3ee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd3ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
    "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
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
    "priority": 8,
    "limit": 5
  }
}
```



