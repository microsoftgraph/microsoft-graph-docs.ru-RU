---
title: Список Енроллментрестриктионсконфигуратионполицисетитемс
description: Список свойств и связей объектов Енроллментрестриктионсконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6f6929b276d7642377d20114ceaf35d204e2e0a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941171"
---
# <a name="list-enrollmentrestrictionsconfigurationpolicysetitems"></a><span data-ttu-id="9477a-103">Список Енроллментрестриктионсконфигуратионполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="9477a-103">List enrollmentRestrictionsConfigurationPolicySetItems</span></span>

> <span data-ttu-id="9477a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9477a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9477a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9477a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9477a-106">Список свойств и связей объектов [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="9477a-106">List properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9477a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9477a-107">Prerequisites</span></span>
<span data-ttu-id="9477a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9477a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9477a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9477a-110">Permission type</span></span>|<span data-ttu-id="9477a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9477a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9477a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9477a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9477a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9477a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9477a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9477a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9477a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9477a-115">Not supported.</span></span>|
|<span data-ttu-id="9477a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9477a-116">Application</span></span>|<span data-ttu-id="9477a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9477a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9477a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9477a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="9477a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9477a-119">Request headers</span></span>
|<span data-ttu-id="9477a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9477a-120">Header</span></span>|<span data-ttu-id="9477a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9477a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9477a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9477a-122">Authorization</span></span>|<span data-ttu-id="9477a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9477a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9477a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9477a-124">Accept</span></span>|<span data-ttu-id="9477a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9477a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9477a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9477a-126">Request body</span></span>
<span data-ttu-id="9477a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9477a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9477a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9477a-128">Response</span></span>
<span data-ttu-id="9477a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9477a-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9477a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9477a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9477a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9477a-131">Request</span></span>
<span data-ttu-id="9477a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9477a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="9477a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9477a-133">Response</span></span>
<span data-ttu-id="9477a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9477a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
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
  ]
}
```





