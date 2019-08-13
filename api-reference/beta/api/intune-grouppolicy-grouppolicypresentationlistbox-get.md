---
title: Получение Граупполиципресентатионлистбокс
description: Чтение свойств и связей объекта Граупполиципресентатионлистбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8587f9def83a05d39ad89dae695b0f4c7a0a6312
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357798"
---
# <a name="get-grouppolicypresentationlistbox"></a><span data-ttu-id="1ca33-103">Получение Граупполиципресентатионлистбокс</span><span class="sxs-lookup"><span data-stu-id="1ca33-103">Get groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="1ca33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ca33-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ca33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ca33-106">Чтение свойств и связей объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="1ca33-106">Read properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ca33-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ca33-107">Prerequisites</span></span>
<span data-ttu-id="1ca33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca33-110">Permission type</span></span>|<span data-ttu-id="1ca33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ca33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ca33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ca33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ca33-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ca33-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1ca33-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ca33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ca33-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca33-115">Not supported.</span></span>|
|<span data-ttu-id="1ca33-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ca33-116">Application</span></span>|<span data-ttu-id="1ca33-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ca33-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ca33-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ca33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ca33-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ca33-119">Optional query parameters</span></span>
<span data-ttu-id="1ca33-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1ca33-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ca33-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ca33-121">Request headers</span></span>
|<span data-ttu-id="1ca33-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ca33-122">Header</span></span>|<span data-ttu-id="1ca33-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1ca33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ca33-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ca33-124">Authorization</span></span>|<span data-ttu-id="1ca33-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ca33-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1ca33-126">Accept</span></span>|<span data-ttu-id="1ca33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1ca33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ca33-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ca33-128">Request body</span></span>
<span data-ttu-id="1ca33-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ca33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ca33-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ca33-130">Response</span></span>
<span data-ttu-id="1ca33-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca33-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ca33-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1ca33-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ca33-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ca33-133">Request</span></span>
<span data-ttu-id="1ca33-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ca33-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="1ca33-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca33-135">Response</span></span>
<span data-ttu-id="1ca33-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ca33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
    "label": "Label value",
    "id": "2e074c87-4c87-2e07-874c-072e874c072e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "explicitValue": true,
    "valuePrefix": "Value Prefix value"
  }
}
```






