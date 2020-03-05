---
title: Список Граупполиципресентатионвалуелистс
description: Список свойств и связей объектов Граупполиципресентатионвалуелист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5790d2ed3fab29747b3d4872388c7c4e73953754
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464199"
---
# <a name="list-grouppolicypresentationvaluelists"></a><span data-ttu-id="26a73-103">Список Граупполиципресентатионвалуелистс</span><span class="sxs-lookup"><span data-stu-id="26a73-103">List groupPolicyPresentationValueLists</span></span>

<span data-ttu-id="26a73-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="26a73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26a73-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a73-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26a73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a73-107">Список свойств и связей объектов [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) .</span><span class="sxs-lookup"><span data-stu-id="26a73-107">List properties and relationships of the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a73-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26a73-108">Prerequisites</span></span>
<span data-ttu-id="26a73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26a73-111">Permission type</span></span>|<span data-ttu-id="26a73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26a73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26a73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26a73-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="26a73-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="26a73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26a73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a73-116">Not supported.</span></span>|
|<span data-ttu-id="26a73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26a73-117">Application</span></span>|<span data-ttu-id="26a73-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="26a73-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26a73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="26a73-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26a73-120">Request headers</span></span>
|<span data-ttu-id="26a73-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26a73-121">Header</span></span>|<span data-ttu-id="26a73-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26a73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a73-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26a73-123">Authorization</span></span>|<span data-ttu-id="26a73-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26a73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26a73-125">Accept</span></span>|<span data-ttu-id="26a73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26a73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a73-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26a73-127">Request body</span></span>
<span data-ttu-id="26a73-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26a73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26a73-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="26a73-129">Response</span></span>
<span data-ttu-id="26a73-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионвалуелист](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26a73-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a73-131">Пример</span><span class="sxs-lookup"><span data-stu-id="26a73-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a73-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26a73-132">Request</span></span>
<span data-ttu-id="26a73-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26a73-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="26a73-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a73-134">Response</span></span>
<span data-ttu-id="26a73-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26a73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
      "values": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```





