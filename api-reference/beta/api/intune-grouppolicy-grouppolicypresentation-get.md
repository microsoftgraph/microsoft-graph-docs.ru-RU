---
title: Получение Граупполиципресентатион
description: Чтение свойств и связей объекта Граупполиципресентатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2bef35f93ac7244c0df963b9a0247c0fedac283
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184152"
---
# <a name="get-grouppolicypresentation"></a><span data-ttu-id="4e3ee-103">Получение Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="4e3ee-103">Get groupPolicyPresentation</span></span>

> <span data-ttu-id="4e3ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e3ee-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e3ee-106">Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="4e3ee-106">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e3ee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e3ee-107">Prerequisites</span></span>
<span data-ttu-id="4e3ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e3ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e3ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e3ee-110">Permission type</span></span>|<span data-ttu-id="4e3ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e3ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e3ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e3ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e3ee-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e3ee-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4e3ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e3ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e3ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-115">Not supported.</span></span>|
|<span data-ttu-id="4e3ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e3ee-116">Application</span></span>|<span data-ttu-id="4e3ee-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e3ee-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e3ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e3ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e3ee-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e3ee-119">Optional query parameters</span></span>
<span data-ttu-id="4e3ee-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e3ee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e3ee-121">Request headers</span></span>
|<span data-ttu-id="4e3ee-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e3ee-122">Header</span></span>|<span data-ttu-id="4e3ee-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4e3ee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e3ee-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e3ee-124">Authorization</span></span>|<span data-ttu-id="4e3ee-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e3ee-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4e3ee-126">Accept</span></span>|<span data-ttu-id="4e3ee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4e3ee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e3ee-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e3ee-128">Request body</span></span>
<span data-ttu-id="4e3ee-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e3ee-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e3ee-130">Response</span></span>
<span data-ttu-id="4e3ee-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e3ee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4e3ee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e3ee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e3ee-133">Request</span></span>
<span data-ttu-id="4e3ee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="4e3ee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e3ee-135">Response</span></span>
<span data-ttu-id="4e3ee-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e3ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentation",
    "label": "Label value",
    "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




