---
title: Получение Граупполиципресентатионтекст
description: Чтение свойств и связей объекта Граупполиципресентатионтекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 134cbb4b3abca0c7200a901de8fb683ac280abea
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194042"
---
# <a name="get-grouppolicypresentationtext"></a><span data-ttu-id="fe958-103">Получение Граупполиципресентатионтекст</span><span class="sxs-lookup"><span data-stu-id="fe958-103">Get groupPolicyPresentationText</span></span>

> <span data-ttu-id="fe958-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe958-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe958-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe958-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe958-106">Чтение свойств и связей объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="fe958-106">Read properties and relationships of the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe958-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe958-107">Prerequisites</span></span>
<span data-ttu-id="fe958-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe958-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe958-110">Permission type</span></span>|<span data-ttu-id="fe958-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe958-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe958-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe958-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe958-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe958-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fe958-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe958-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe958-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe958-115">Not supported.</span></span>|
|<span data-ttu-id="fe958-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe958-116">Application</span></span>|<span data-ttu-id="fe958-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe958-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe958-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe958-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe958-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe958-119">Optional query parameters</span></span>
<span data-ttu-id="fe958-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe958-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe958-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe958-121">Request headers</span></span>
|<span data-ttu-id="fe958-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe958-122">Header</span></span>|<span data-ttu-id="fe958-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fe958-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe958-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe958-124">Authorization</span></span>|<span data-ttu-id="fe958-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe958-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe958-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fe958-126">Accept</span></span>|<span data-ttu-id="fe958-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fe958-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe958-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe958-128">Request body</span></span>
<span data-ttu-id="fe958-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe958-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe958-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe958-130">Response</span></span>
<span data-ttu-id="fe958-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe958-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe958-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fe958-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe958-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe958-133">Request</span></span>
<span data-ttu-id="fe958-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe958-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="fe958-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe958-135">Response</span></span>
<span data-ttu-id="fe958-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe958-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
    "label": "Label value",
    "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




