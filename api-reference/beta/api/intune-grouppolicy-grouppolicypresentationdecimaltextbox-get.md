---
title: Получение ГраупполиципресентатиондеЦималтекстбокс
description: Чтение свойств и связей объекта ГраупполиципресентатиондеЦималтекстбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c91830d374ed509bdb62ebcc4373c2ce42cba5a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942999"
---
# <a name="get-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="8c6ae-103">Получение ГраупполиципресентатиондеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="8c6ae-103">Get groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="8c6ae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c6ae-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6ae-106">Чтение свойств и связей объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="8c6ae-106">Read properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c6ae-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c6ae-107">Prerequisites</span></span>
<span data-ttu-id="8c6ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c6ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c6ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c6ae-110">Permission type</span></span>|<span data-ttu-id="8c6ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c6ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c6ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c6ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c6ae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c6ae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8c6ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c6ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c6ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-115">Not supported.</span></span>|
|<span data-ttu-id="8c6ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c6ae-116">Application</span></span>|<span data-ttu-id="8c6ae-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c6ae-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c6ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c6ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c6ae-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c6ae-119">Optional query parameters</span></span>
<span data-ttu-id="8c6ae-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c6ae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c6ae-121">Request headers</span></span>
|<span data-ttu-id="8c6ae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c6ae-122">Header</span></span>|<span data-ttu-id="8c6ae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8c6ae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c6ae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c6ae-124">Authorization</span></span>|<span data-ttu-id="8c6ae-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c6ae-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8c6ae-126">Accept</span></span>|<span data-ttu-id="8c6ae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8c6ae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c6ae-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c6ae-128">Request body</span></span>
<span data-ttu-id="8c6ae-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c6ae-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c6ae-130">Response</span></span>
<span data-ttu-id="8c6ae-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c6ae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8c6ae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c6ae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c6ae-133">Request</span></span>
<span data-ttu-id="8c6ae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="8c6ae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c6ae-135">Response</span></span>
<span data-ttu-id="8c6ae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c6ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





