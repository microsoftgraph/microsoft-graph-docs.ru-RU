---
title: Get groupPolicyPresentation
description: Чтение свойств и связей объекта groupPolicyPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 088afc48890b567b86f786995a2dc2d11d3c712d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142011"
---
# <a name="get-grouppolicypresentation"></a><span data-ttu-id="a7754-103">Get groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="a7754-103">Get groupPolicyPresentation</span></span>

<span data-ttu-id="a7754-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7754-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7754-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7754-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7754-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7754-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7754-107">Чтение свойств и связей объекта [groupPolicyPresentation.](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a7754-107">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7754-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7754-108">Prerequisites</span></span>
<span data-ttu-id="a7754-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7754-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7754-111">Permission type</span></span>|<span data-ttu-id="a7754-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7754-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7754-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7754-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7754-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7754-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7754-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7754-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7754-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7754-116">Not supported.</span></span>|
|<span data-ttu-id="a7754-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7754-117">Application</span></span>|<span data-ttu-id="a7754-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7754-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7754-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7754-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7754-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7754-120">Optional query parameters</span></span>
<span data-ttu-id="a7754-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a7754-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7754-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7754-122">Request headers</span></span>
|<span data-ttu-id="a7754-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7754-123">Header</span></span>|<span data-ttu-id="a7754-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a7754-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7754-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7754-125">Authorization</span></span>|<span data-ttu-id="a7754-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7754-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7754-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a7754-127">Accept</span></span>|<span data-ttu-id="a7754-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a7754-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7754-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7754-129">Request body</span></span>
<span data-ttu-id="a7754-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7754-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7754-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7754-131">Response</span></span>
<span data-ttu-id="a7754-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7754-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7754-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a7754-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7754-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7754-134">Request</span></span>
<span data-ttu-id="a7754-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7754-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="a7754-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7754-136">Response</span></span>
<span data-ttu-id="a7754-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7754-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




