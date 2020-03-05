---
title: Получение Граупполиципресентатионкомбобокс
description: Чтение свойств и связей объекта Граупполиципресентатионкомбобокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ccd7029bdef05e71fa2e9678167712e6503ed4dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464920"
---
# <a name="get-grouppolicypresentationcombobox"></a><span data-ttu-id="ffbfa-103">Получение Граупполиципресентатионкомбобокс</span><span class="sxs-lookup"><span data-stu-id="ffbfa-103">Get groupPolicyPresentationComboBox</span></span>

<span data-ttu-id="ffbfa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ffbfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffbfa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffbfa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffbfa-107">Чтение свойств и связей объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="ffbfa-107">Read properties and relationships of the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffbfa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ffbfa-108">Prerequisites</span></span>
<span data-ttu-id="ffbfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffbfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffbfa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffbfa-111">Permission type</span></span>|<span data-ttu-id="ffbfa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffbfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffbfa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffbfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffbfa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffbfa-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ffbfa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffbfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffbfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-116">Not supported.</span></span>|
|<span data-ttu-id="ffbfa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffbfa-117">Application</span></span>|<span data-ttu-id="ffbfa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffbfa-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffbfa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffbfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffbfa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffbfa-120">Optional query parameters</span></span>
<span data-ttu-id="ffbfa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffbfa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffbfa-122">Request headers</span></span>
|<span data-ttu-id="ffbfa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffbfa-123">Header</span></span>|<span data-ttu-id="ffbfa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ffbfa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffbfa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffbfa-125">Authorization</span></span>|<span data-ttu-id="ffbfa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffbfa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ffbfa-127">Accept</span></span>|<span data-ttu-id="ffbfa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ffbfa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffbfa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffbfa-129">Request body</span></span>
<span data-ttu-id="ffbfa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffbfa-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffbfa-131">Response</span></span>
<span data-ttu-id="ffbfa-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffbfa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ffbfa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffbfa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffbfa-134">Request</span></span>
<span data-ttu-id="ffbfa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="ffbfa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffbfa-136">Response</span></span>
<span data-ttu-id="ffbfa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffbfa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
    "label": "Label value",
    "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": "Default Value value",
    "suggestions": [
      "Suggestions value"
    ],
    "required": true,
    "maxLength": 9
  }
}
```





