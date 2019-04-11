---
title: Список Граупполиципресентатионлистбоксес
description: Список свойств и связей объектов Граупполиципресентатионлистбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36744bc759fb972423e98b209c1c006f59472c5d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784336"
---
# <a name="list-grouppolicypresentationlistboxes"></a><span data-ttu-id="421a9-103">Список Граупполиципресентатионлистбоксес</span><span class="sxs-lookup"><span data-stu-id="421a9-103">List groupPolicyPresentationListBoxes</span></span>

> <span data-ttu-id="421a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421a9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="421a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421a9-106">Список свойств и связей объектов [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="421a9-106">List properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="421a9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="421a9-107">Prerequisites</span></span>
<span data-ttu-id="421a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="421a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="421a9-110">Permission type</span></span>|<span data-ttu-id="421a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="421a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="421a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="421a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="421a9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="421a9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="421a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="421a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="421a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421a9-115">Not supported.</span></span>|
|<span data-ttu-id="421a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="421a9-116">Application</span></span>|<span data-ttu-id="421a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="421a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="421a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="421a9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="421a9-119">Request headers</span></span>
|<span data-ttu-id="421a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="421a9-120">Header</span></span>|<span data-ttu-id="421a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="421a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="421a9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="421a9-122">Authorization</span></span>|<span data-ttu-id="421a9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="421a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="421a9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="421a9-124">Accept</span></span>|<span data-ttu-id="421a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="421a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="421a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="421a9-126">Request body</span></span>
<span data-ttu-id="421a9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="421a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="421a9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="421a9-128">Response</span></span>
<span data-ttu-id="421a9-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="421a9-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="421a9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="421a9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="421a9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="421a9-131">Request</span></span>
<span data-ttu-id="421a9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="421a9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="421a9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="421a9-133">Response</span></span>
<span data-ttu-id="421a9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="421a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
      "label": "Label value",
      "id": "2e074c87-4c87-2e07-874c-072e874c072e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "explicitValue": true
    }
  ]
}
```





