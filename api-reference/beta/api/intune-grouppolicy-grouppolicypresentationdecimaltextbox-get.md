---
title: Get groupPolicyPresentationDecimalTextBox
description: Чтение свойств и связей объекта groupPolicyPresentationDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 375694abdae02e5f64e1f22279fe748c438840aa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149655"
---
# <a name="get-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="22cb1-103">Get groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="22cb1-103">Get groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="22cb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22cb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22cb1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22cb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22cb1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22cb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22cb1-107">Чтение свойств и связей объекта [groupPolicyPresentationDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="22cb1-107">Read properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22cb1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22cb1-108">Prerequisites</span></span>
<span data-ttu-id="22cb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22cb1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22cb1-111">Permission type</span></span>|<span data-ttu-id="22cb1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22cb1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22cb1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22cb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22cb1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cb1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22cb1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22cb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22cb1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22cb1-116">Not supported.</span></span>|
|<span data-ttu-id="22cb1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="22cb1-117">Application</span></span>|<span data-ttu-id="22cb1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cb1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22cb1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22cb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22cb1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22cb1-120">Optional query parameters</span></span>
<span data-ttu-id="22cb1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22cb1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22cb1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22cb1-122">Request headers</span></span>
|<span data-ttu-id="22cb1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22cb1-123">Header</span></span>|<span data-ttu-id="22cb1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="22cb1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22cb1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="22cb1-125">Authorization</span></span>|<span data-ttu-id="22cb1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22cb1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22cb1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="22cb1-127">Accept</span></span>|<span data-ttu-id="22cb1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="22cb1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22cb1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22cb1-129">Request body</span></span>
<span data-ttu-id="22cb1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22cb1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22cb1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cb1-131">Response</span></span>
<span data-ttu-id="22cb1-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="22cb1-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22cb1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="22cb1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="22cb1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="22cb1-134">Request</span></span>
<span data-ttu-id="22cb1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22cb1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="22cb1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cb1-136">Response</span></span>
<span data-ttu-id="22cb1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22cb1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
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
}
```




