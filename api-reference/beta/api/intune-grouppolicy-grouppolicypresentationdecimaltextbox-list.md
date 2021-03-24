---
title: List groupPolicyPresentationDecimalTextBoxes
description: Список свойств и связей объектов groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2141c03b02a38bec55497e6eb4362f1d9f6253f5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149641"
---
# <a name="list-grouppolicypresentationdecimaltextboxes"></a><span data-ttu-id="e8087-103">List groupPolicyPresentationDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="e8087-103">List groupPolicyPresentationDecimalTextBoxes</span></span>

<span data-ttu-id="e8087-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8087-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8087-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8087-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8087-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8087-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8087-107">Список свойств и связей объектов [groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="e8087-107">List properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8087-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8087-108">Prerequisites</span></span>
<span data-ttu-id="e8087-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8087-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8087-111">Permission type</span></span>|<span data-ttu-id="e8087-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8087-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8087-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8087-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8087-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8087-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8087-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8087-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8087-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8087-116">Not supported.</span></span>|
|<span data-ttu-id="e8087-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8087-117">Application</span></span>|<span data-ttu-id="e8087-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8087-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8087-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8087-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="e8087-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8087-120">Request headers</span></span>
|<span data-ttu-id="e8087-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8087-121">Header</span></span>|<span data-ttu-id="e8087-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8087-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8087-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8087-123">Authorization</span></span>|<span data-ttu-id="e8087-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8087-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8087-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8087-125">Accept</span></span>|<span data-ttu-id="e8087-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8087-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8087-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8087-127">Request body</span></span>
<span data-ttu-id="e8087-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8087-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8087-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8087-129">Response</span></span>
<span data-ttu-id="e8087-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8087-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8087-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e8087-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8087-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8087-132">Request</span></span>
<span data-ttu-id="e8087-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8087-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="e8087-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8087-134">Response</span></span>
<span data-ttu-id="e8087-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8087-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
      "label": "Label value",
      "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultValue": 12,
      "spin": true,
      "spinStep": 8,
      "required": true,
      "minValue": 8,
      "maxValue": 8
    }
  ]
}
```




