---
title: Список ГраупполиципресентатионлонгдеЦималтекстбоксес
description: Список свойств и связей объектов ГраупполиципресентатионлонгдеЦималтекстбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e1e9791e42af0e1b848da496154f16e3acf2b0b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964614"
---
# <a name="list-grouppolicypresentationlongdecimaltextboxes"></a><span data-ttu-id="7fb83-103">Список ГраупполиципресентатионлонгдеЦималтекстбоксес</span><span class="sxs-lookup"><span data-stu-id="7fb83-103">List groupPolicyPresentationLongDecimalTextBoxes</span></span>

> <span data-ttu-id="7fb83-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fb83-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fb83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fb83-106">Список свойств и связей объектов [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="7fb83-106">List properties and relationships of the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fb83-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7fb83-107">Prerequisites</span></span>
<span data-ttu-id="7fb83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fb83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb83-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb83-110">Permission type</span></span>|<span data-ttu-id="7fb83-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fb83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb83-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fb83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb83-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fb83-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7fb83-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fb83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb83-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb83-115">Not supported.</span></span>|
|<span data-ttu-id="7fb83-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fb83-116">Application</span></span>|<span data-ttu-id="7fb83-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb83-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fb83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7fb83-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fb83-119">Request headers</span></span>
|<span data-ttu-id="7fb83-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fb83-120">Header</span></span>|<span data-ttu-id="7fb83-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7fb83-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb83-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fb83-122">Authorization</span></span>|<span data-ttu-id="7fb83-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fb83-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fb83-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7fb83-124">Accept</span></span>|<span data-ttu-id="7fb83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb83-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb83-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fb83-126">Request body</span></span>
<span data-ttu-id="7fb83-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fb83-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb83-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb83-128">Response</span></span>
<span data-ttu-id="7fb83-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fb83-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb83-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7fb83-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fb83-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fb83-131">Request</span></span>
<span data-ttu-id="7fb83-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fb83-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="7fb83-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fb83-133">Response</span></span>
<span data-ttu-id="7fb83-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fb83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
      "label": "Label value",
      "id": "754d8495-8495-754d-9584-4d7595844d75",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultValue": 12,
      "spin": true,
      "spinStep": 8,
      "required": true,
      "minValue": 8,
      "maxValue": 8
    }
  ]
}
```





