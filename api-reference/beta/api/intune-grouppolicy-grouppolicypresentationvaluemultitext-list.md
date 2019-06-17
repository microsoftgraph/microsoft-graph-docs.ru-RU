---
title: Список Граупполиципресентатионвалуемултитекстс
description: Список свойств и связей объектов Граупполиципресентатионвалуемултитекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 802efde25c889b7e68649ede6ed192534bd58823
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985782"
---
# <a name="list-grouppolicypresentationvaluemultitexts"></a><span data-ttu-id="e2859-103">Список Граупполиципресентатионвалуемултитекстс</span><span class="sxs-lookup"><span data-stu-id="e2859-103">List groupPolicyPresentationValueMultiTexts</span></span>

> <span data-ttu-id="e2859-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2859-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2859-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2859-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2859-106">Список свойств и связей объектов [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="e2859-106">List properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2859-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2859-107">Prerequisites</span></span>
<span data-ttu-id="e2859-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2859-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2859-110">Permission type</span></span>|<span data-ttu-id="e2859-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2859-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2859-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2859-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2859-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e2859-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2859-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2859-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2859-115">Not supported.</span></span>|
|<span data-ttu-id="e2859-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2859-116">Application</span></span>|<span data-ttu-id="e2859-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2859-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2859-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2859-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="e2859-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2859-119">Request headers</span></span>
|<span data-ttu-id="e2859-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2859-120">Header</span></span>|<span data-ttu-id="e2859-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e2859-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2859-122">Authorization</span></span>|<span data-ttu-id="e2859-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2859-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2859-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e2859-124">Accept</span></span>|<span data-ttu-id="e2859-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2859-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2859-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2859-126">Request body</span></span>
<span data-ttu-id="e2859-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2859-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2859-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2859-128">Response</span></span>
<span data-ttu-id="e2859-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2859-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2859-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e2859-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2859-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2859-131">Request</span></span>
<span data-ttu-id="e2859-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2859-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="e2859-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2859-133">Response</span></span>
<span data-ttu-id="e2859-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2859-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "5156903b-903b-5156-3b90-56513b905651",
      "values": [
        "Values value"
      ]
    }
  ]
}
```





