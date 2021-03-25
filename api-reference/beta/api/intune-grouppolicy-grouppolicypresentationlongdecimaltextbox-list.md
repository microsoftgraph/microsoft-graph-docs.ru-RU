---
title: List groupPolicyPresentationLongDecimalTextBoxes
description: Список свойств и связей объектов groupPolicyPresentationLongDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9778373bc3e9b7b931a093c0ffcae22d2e70c409
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153281"
---
# <a name="list-grouppolicypresentationlongdecimaltextboxes"></a><span data-ttu-id="37600-103">List groupPolicyPresentationLongDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="37600-103">List groupPolicyPresentationLongDecimalTextBoxes</span></span>

<span data-ttu-id="37600-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37600-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37600-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37600-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37600-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37600-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37600-107">Список свойств и связей объектов [groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="37600-107">List properties and relationships of the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37600-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37600-108">Prerequisites</span></span>
<span data-ttu-id="37600-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37600-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37600-111">Permission type</span></span>|<span data-ttu-id="37600-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37600-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37600-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37600-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37600-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37600-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37600-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37600-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37600-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37600-116">Not supported.</span></span>|
|<span data-ttu-id="37600-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="37600-117">Application</span></span>|<span data-ttu-id="37600-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37600-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37600-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37600-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="37600-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37600-120">Request headers</span></span>
|<span data-ttu-id="37600-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37600-121">Header</span></span>|<span data-ttu-id="37600-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37600-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37600-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37600-123">Authorization</span></span>|<span data-ttu-id="37600-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37600-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37600-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37600-125">Accept</span></span>|<span data-ttu-id="37600-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37600-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37600-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37600-127">Request body</span></span>
<span data-ttu-id="37600-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37600-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37600-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="37600-129">Response</span></span>
<span data-ttu-id="37600-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37600-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37600-131">Пример</span><span class="sxs-lookup"><span data-stu-id="37600-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="37600-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="37600-132">Request</span></span>
<span data-ttu-id="37600-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37600-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="37600-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37600-134">Response</span></span>
<span data-ttu-id="37600-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37600-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
      "label": "Label value",
      "id": "754d8495-8495-754d-9584-4d7595844d75",
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




