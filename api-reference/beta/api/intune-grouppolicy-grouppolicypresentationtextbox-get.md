---
title: Получение Граупполиципресентатионтекстбокс
description: Чтение свойств и связей объекта Граупполиципресентатионтекстбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86cb83a57a26f6fc60cfe2c7e6f62fc178874d2d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904652"
---
# <a name="get-grouppolicypresentationtextbox"></a><span data-ttu-id="eb433-103">Получение Граупполиципресентатионтекстбокс</span><span class="sxs-lookup"><span data-stu-id="eb433-103">Get groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="eb433-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb433-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb433-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb433-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb433-106">Чтение свойств и связей объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="eb433-106">Read properties and relationships of the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb433-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb433-107">Prerequisites</span></span>
<span data-ttu-id="eb433-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb433-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb433-110">Permission type</span></span>|<span data-ttu-id="eb433-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb433-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb433-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb433-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb433-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb433-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="eb433-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb433-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb433-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb433-115">Not supported.</span></span>|
|<span data-ttu-id="eb433-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb433-116">Application</span></span>|<span data-ttu-id="eb433-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb433-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb433-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb433-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb433-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb433-119">Optional query parameters</span></span>
<span data-ttu-id="eb433-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb433-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb433-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb433-121">Request headers</span></span>
|<span data-ttu-id="eb433-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb433-122">Header</span></span>|<span data-ttu-id="eb433-123">Значение</span><span class="sxs-lookup"><span data-stu-id="eb433-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb433-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb433-124">Authorization</span></span>|<span data-ttu-id="eb433-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb433-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb433-126">Accept</span><span class="sxs-lookup"><span data-stu-id="eb433-126">Accept</span></span>|<span data-ttu-id="eb433-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb433-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb433-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb433-128">Request body</span></span>
<span data-ttu-id="eb433-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb433-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb433-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb433-130">Response</span></span>
<span data-ttu-id="eb433-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb433-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb433-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eb433-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb433-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb433-133">Request</span></span>
<span data-ttu-id="eb433-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb433-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="eb433-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb433-135">Response</span></span>
<span data-ttu-id="eb433-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb433-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
    "label": "Label value",
    "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultValue": "Default Value value",
    "required": true,
    "maxLength": 9
  }
}
```




