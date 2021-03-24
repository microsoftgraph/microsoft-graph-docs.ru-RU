---
title: Регистрация спискаRestrictionsConfigurationPolicySetItems
description: Список свойств и связей объектов enrollmentRestrictionsConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca3df0957405890ec2f62dc73fc88678fc01ead6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148611"
---
# <a name="list-enrollmentrestrictionsconfigurationpolicysetitems"></a><span data-ttu-id="23239-103">Регистрация спискаRestrictionsConfigurationPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="23239-103">List enrollmentRestrictionsConfigurationPolicySetItems</span></span>

<span data-ttu-id="23239-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23239-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23239-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23239-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23239-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23239-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23239-107">Список свойств и связей объектов [enrollmentRestrictionsConfigurationPolicySetItem.](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="23239-107">List properties and relationships of the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23239-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23239-108">Prerequisites</span></span>
<span data-ttu-id="23239-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23239-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23239-111">Permission type</span></span>|<span data-ttu-id="23239-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23239-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23239-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23239-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23239-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23239-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23239-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23239-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23239-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23239-116">Not supported.</span></span>|
|<span data-ttu-id="23239-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="23239-117">Application</span></span>|<span data-ttu-id="23239-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23239-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23239-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23239-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="23239-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="23239-120">Request headers</span></span>
|<span data-ttu-id="23239-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23239-121">Header</span></span>|<span data-ttu-id="23239-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23239-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23239-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23239-123">Authorization</span></span>|<span data-ttu-id="23239-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23239-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23239-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23239-125">Accept</span></span>|<span data-ttu-id="23239-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23239-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23239-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23239-127">Request body</span></span>
<span data-ttu-id="23239-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23239-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23239-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="23239-129">Response</span></span>
<span data-ttu-id="23239-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="23239-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23239-131">Пример</span><span class="sxs-lookup"><span data-stu-id="23239-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="23239-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="23239-132">Request</span></span>
<span data-ttu-id="23239-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23239-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="23239-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="23239-134">Response</span></span>
<span data-ttu-id="23239-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23239-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




