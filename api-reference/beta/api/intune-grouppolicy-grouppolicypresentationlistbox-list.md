---
title: Список Граупполиципресентатионлистбоксес
description: Список свойств и связей объектов Граупполиципресентатионлистбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84a8b4f68f464ba32bbd7c8031378d71276020e8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49227583"
---
# <a name="list-grouppolicypresentationlistboxes"></a><span data-ttu-id="e97ea-103">Список Граупполиципресентатионлистбоксес</span><span class="sxs-lookup"><span data-stu-id="e97ea-103">List groupPolicyPresentationListBoxes</span></span>

<span data-ttu-id="e97ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e97ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e97ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e97ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e97ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e97ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e97ea-107">Список свойств и связей объектов [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="e97ea-107">List properties and relationships of the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e97ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e97ea-108">Prerequisites</span></span>
<span data-ttu-id="e97ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e97ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e97ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e97ea-111">Permission type</span></span>|<span data-ttu-id="e97ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e97ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e97ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e97ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e97ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e97ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e97ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e97ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e97ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e97ea-116">Not supported.</span></span>|
|<span data-ttu-id="e97ea-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e97ea-117">Application</span></span>|<span data-ttu-id="e97ea-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e97ea-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e97ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e97ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="e97ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e97ea-120">Request headers</span></span>
|<span data-ttu-id="e97ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e97ea-121">Header</span></span>|<span data-ttu-id="e97ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e97ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e97ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e97ea-123">Authorization</span></span>|<span data-ttu-id="e97ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e97ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e97ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e97ea-125">Accept</span></span>|<span data-ttu-id="e97ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e97ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e97ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e97ea-127">Request body</span></span>
<span data-ttu-id="e97ea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e97ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e97ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e97ea-129">Response</span></span>
<span data-ttu-id="e97ea-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e97ea-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e97ea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e97ea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e97ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e97ea-132">Request</span></span>
<span data-ttu-id="e97ea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e97ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="e97ea-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e97ea-134">Response</span></span>
<span data-ttu-id="e97ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e97ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 335

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
      "label": "Label value",
      "id": "2e074c87-4c87-2e07-874c-072e874c072e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "explicitValue": true,
      "valuePrefix": "Value Prefix value"
    }
  ]
}
```




