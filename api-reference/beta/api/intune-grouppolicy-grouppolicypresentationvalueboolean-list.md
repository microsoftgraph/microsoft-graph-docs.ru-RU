---
title: Список Граупполиципресентатионвалуебулеанс
description: Список свойств и связей объектов Граупполиципресентатионвалуебулеан.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5541e39fea611e8d3e1d42ed74e82d184c5214f4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464283"
---
# <a name="list-grouppolicypresentationvaluebooleans"></a><span data-ttu-id="64322-103">Список Граупполиципресентатионвалуебулеанс</span><span class="sxs-lookup"><span data-stu-id="64322-103">List groupPolicyPresentationValueBooleans</span></span>

<span data-ttu-id="64322-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64322-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64322-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64322-107">Список свойств и связей объектов [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) .</span><span class="sxs-lookup"><span data-stu-id="64322-107">List properties and relationships of the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64322-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64322-108">Prerequisites</span></span>
<span data-ttu-id="64322-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64322-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64322-111">Permission type</span></span>|<span data-ttu-id="64322-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64322-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64322-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64322-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64322-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64322-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="64322-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64322-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64322-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64322-116">Not supported.</span></span>|
|<span data-ttu-id="64322-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64322-117">Application</span></span>|<span data-ttu-id="64322-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64322-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64322-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64322-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="64322-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64322-120">Request headers</span></span>
|<span data-ttu-id="64322-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64322-121">Header</span></span>|<span data-ttu-id="64322-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64322-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64322-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64322-123">Authorization</span></span>|<span data-ttu-id="64322-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64322-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64322-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64322-125">Accept</span></span>|<span data-ttu-id="64322-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64322-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64322-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64322-127">Request body</span></span>
<span data-ttu-id="64322-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64322-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64322-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="64322-129">Response</span></span>
<span data-ttu-id="64322-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионвалуебулеан](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64322-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64322-131">Пример</span><span class="sxs-lookup"><span data-stu-id="64322-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64322-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="64322-132">Request</span></span>
<span data-ttu-id="64322-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64322-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="64322-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="64322-134">Response</span></span>
<span data-ttu-id="64322-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64322-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "be61344f-344f-be61-4f34-61be4f3461be",
      "value": true
    }
  ]
}
```





