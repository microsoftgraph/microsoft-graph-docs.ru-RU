---
title: Get groupPolicyPresentationValueBoolean
description: Чтение свойств и связей объекта groupPolicyPresentationValueBoolean.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a60c21e771e7baaecb8045e65d77072ede33d7f6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157264"
---
# <a name="get-grouppolicypresentationvalueboolean"></a><span data-ttu-id="1ba92-103">Get groupPolicyPresentationValueBoolean</span><span class="sxs-lookup"><span data-stu-id="1ba92-103">Get groupPolicyPresentationValueBoolean</span></span>

<span data-ttu-id="1ba92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ba92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ba92-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ba92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ba92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ba92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ba92-107">Чтение свойств и связей объекта [groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)</span><span class="sxs-lookup"><span data-stu-id="1ba92-107">Read properties and relationships of the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ba92-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ba92-108">Prerequisites</span></span>
<span data-ttu-id="1ba92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ba92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ba92-111">Permission type</span></span>|<span data-ttu-id="1ba92-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ba92-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ba92-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ba92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ba92-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba92-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ba92-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ba92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ba92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ba92-116">Not supported.</span></span>|
|<span data-ttu-id="1ba92-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1ba92-117">Application</span></span>|<span data-ttu-id="1ba92-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba92-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ba92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ba92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ba92-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ba92-120">Optional query parameters</span></span>
<span data-ttu-id="1ba92-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1ba92-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ba92-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ba92-122">Request headers</span></span>
|<span data-ttu-id="1ba92-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ba92-123">Header</span></span>|<span data-ttu-id="1ba92-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1ba92-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ba92-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba92-125">Authorization</span></span>|<span data-ttu-id="1ba92-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ba92-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ba92-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1ba92-127">Accept</span></span>|<span data-ttu-id="1ba92-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba92-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ba92-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ba92-129">Request body</span></span>
<span data-ttu-id="1ba92-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ba92-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ba92-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ba92-131">Response</span></span>
<span data-ttu-id="1ba92-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1ba92-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ba92-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1ba92-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ba92-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ba92-134">Request</span></span>
<span data-ttu-id="1ba92-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ba92-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="1ba92-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ba92-136">Response</span></span>
<span data-ttu-id="1ba92-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ba92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "be61344f-344f-be61-4f34-61be4f3461be",
    "value": true
  }
}
```




