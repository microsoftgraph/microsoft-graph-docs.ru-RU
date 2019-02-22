---
title: Получение ГраупполиципресентатиондеЦималтекстбокс
description: Чтение свойств и связей объекта ГраупполиципресентатиондеЦималтекстбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3020813dc820a4bbd752d3e70b214e9ddf6b7a9f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169568"
---
# <a name="get-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="89457-103">Получение ГраупполиципресентатиондеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="89457-103">Get groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="89457-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89457-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89457-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89457-106">Чтение свойств и связей объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="89457-106">Read properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89457-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89457-107">Prerequisites</span></span>
<span data-ttu-id="89457-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="89457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="89457-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89457-110">Permission type</span></span>|<span data-ttu-id="89457-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89457-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89457-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89457-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89457-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="89457-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="89457-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89457-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89457-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89457-115">Not supported.</span></span>|
|<span data-ttu-id="89457-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89457-116">Application</span></span>|<span data-ttu-id="89457-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89457-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89457-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89457-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89457-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89457-119">Optional query parameters</span></span>
<span data-ttu-id="89457-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="89457-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89457-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89457-121">Request headers</span></span>
|<span data-ttu-id="89457-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89457-122">Header</span></span>|<span data-ttu-id="89457-123">Значение</span><span class="sxs-lookup"><span data-stu-id="89457-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89457-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89457-124">Authorization</span></span>|<span data-ttu-id="89457-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="89457-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89457-126">Accept</span><span class="sxs-lookup"><span data-stu-id="89457-126">Accept</span></span>|<span data-ttu-id="89457-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89457-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89457-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89457-128">Request body</span></span>
<span data-ttu-id="89457-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89457-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89457-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="89457-130">Response</span></span>
<span data-ttu-id="89457-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89457-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89457-132">Пример</span><span class="sxs-lookup"><span data-stu-id="89457-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="89457-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="89457-133">Request</span></span>
<span data-ttu-id="89457-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89457-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="89457-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="89457-135">Response</span></span>
<span data-ttu-id="89457-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89457-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




