---
title: Политика listSetItems
description: Список свойств и связей объектов policySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1818a935a089bb92ea862d36b8df3a35396881be
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134573"
---
# <a name="list-policysetitems"></a><span data-ttu-id="90ba7-103">Политика listSetItems</span><span class="sxs-lookup"><span data-stu-id="90ba7-103">List policySetItems</span></span>

<span data-ttu-id="90ba7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ba7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90ba7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ba7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ba7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90ba7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ba7-107">Список свойств и связей объектов [policySetItem.](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="90ba7-107">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90ba7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90ba7-108">Prerequisites</span></span>
<span data-ttu-id="90ba7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ba7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90ba7-111">Permission type</span></span>|<span data-ttu-id="90ba7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90ba7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ba7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90ba7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90ba7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ba7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90ba7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90ba7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ba7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ba7-116">Not supported.</span></span>|
|<span data-ttu-id="90ba7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="90ba7-117">Application</span></span>|<span data-ttu-id="90ba7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ba7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ba7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90ba7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="90ba7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90ba7-120">Request headers</span></span>
|<span data-ttu-id="90ba7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90ba7-121">Header</span></span>|<span data-ttu-id="90ba7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90ba7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ba7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90ba7-123">Authorization</span></span>|<span data-ttu-id="90ba7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90ba7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ba7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90ba7-125">Accept</span></span>|<span data-ttu-id="90ba7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90ba7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ba7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90ba7-127">Request body</span></span>
<span data-ttu-id="90ba7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90ba7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90ba7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ba7-129">Response</span></span>
<span data-ttu-id="90ba7-130">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` объектов [policySetItem](../resources/intune-policyset-policysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="90ba7-130">If successful, this method returns a `200 OK` response code and a collection of [policySetItem](../resources/intune-policyset-policysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ba7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90ba7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90ba7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90ba7-132">Request</span></span>
<span data-ttu-id="90ba7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90ba7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="90ba7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90ba7-134">Response</span></span>
<span data-ttu-id="90ba7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90ba7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
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




