---
title: Получение ГраупполиципресентатиондеЦималтекстбокс
description: Чтение свойств и связей объекта ГраупполиципресентатиондеЦималтекстбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11e33f9f0c3e6ad9e75dea547658d22b75c2284e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464801"
---
# <a name="get-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="205f8-103">Получение ГраупполиципресентатиондеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="205f8-103">Get groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="205f8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="205f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="205f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="205f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="205f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="205f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="205f8-107">Чтение свойств и связей объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="205f8-107">Read properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="205f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="205f8-108">Prerequisites</span></span>
<span data-ttu-id="205f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="205f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="205f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="205f8-111">Permission type</span></span>|<span data-ttu-id="205f8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="205f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="205f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="205f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="205f8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="205f8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="205f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="205f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="205f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="205f8-116">Not supported.</span></span>|
|<span data-ttu-id="205f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="205f8-117">Application</span></span>|<span data-ttu-id="205f8-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="205f8-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="205f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="205f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="205f8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="205f8-120">Optional query parameters</span></span>
<span data-ttu-id="205f8-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="205f8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="205f8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="205f8-122">Request headers</span></span>
|<span data-ttu-id="205f8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="205f8-123">Header</span></span>|<span data-ttu-id="205f8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="205f8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="205f8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="205f8-125">Authorization</span></span>|<span data-ttu-id="205f8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="205f8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="205f8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="205f8-127">Accept</span></span>|<span data-ttu-id="205f8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="205f8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="205f8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="205f8-129">Request body</span></span>
<span data-ttu-id="205f8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="205f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="205f8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="205f8-131">Response</span></span>
<span data-ttu-id="205f8-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="205f8-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="205f8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="205f8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="205f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="205f8-134">Request</span></span>
<span data-ttu-id="205f8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="205f8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="205f8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="205f8-136">Response</span></span>
<span data-ttu-id="205f8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="205f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





