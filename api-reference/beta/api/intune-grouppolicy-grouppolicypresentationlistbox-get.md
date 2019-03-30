---
title: Получение Граупполиципресентатионлистбокс
description: Чтение свойств и связей объекта Граупполиципресентатионлистбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ef86bb16320e8a62d9bec6adf278f7904a6c151
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965825"
---
# <a name="get-grouppolicypresentationlistbox"></a><span data-ttu-id="49141-103">Получение Граупполиципресентатионлистбокс</span><span class="sxs-lookup"><span data-stu-id="49141-103">Get groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="49141-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49141-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49141-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49141-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49141-106">Чтение свойств и связей объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="49141-106">Read properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49141-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49141-107">Prerequisites</span></span>
<span data-ttu-id="49141-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49141-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49141-110">Permission type</span></span>|<span data-ttu-id="49141-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49141-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49141-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49141-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49141-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="49141-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="49141-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49141-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49141-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49141-115">Not supported.</span></span>|
|<span data-ttu-id="49141-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49141-116">Application</span></span>|<span data-ttu-id="49141-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49141-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49141-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49141-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49141-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49141-119">Optional query parameters</span></span>
<span data-ttu-id="49141-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49141-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49141-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49141-121">Request headers</span></span>
|<span data-ttu-id="49141-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49141-122">Header</span></span>|<span data-ttu-id="49141-123">Значение</span><span class="sxs-lookup"><span data-stu-id="49141-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49141-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49141-124">Authorization</span></span>|<span data-ttu-id="49141-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49141-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49141-126">Accept</span><span class="sxs-lookup"><span data-stu-id="49141-126">Accept</span></span>|<span data-ttu-id="49141-127">application/json</span><span class="sxs-lookup"><span data-stu-id="49141-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49141-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49141-128">Request body</span></span>
<span data-ttu-id="49141-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49141-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49141-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="49141-130">Response</span></span>
<span data-ttu-id="49141-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49141-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49141-132">Пример</span><span class="sxs-lookup"><span data-stu-id="49141-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="49141-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="49141-133">Request</span></span>
<span data-ttu-id="49141-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49141-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="49141-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="49141-135">Response</span></span>
<span data-ttu-id="49141-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49141-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 267

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
    "label": "Label value",
    "id": "2e074c87-4c87-2e07-874c-072e874c072e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "explicitValue": true
  }
}
```




