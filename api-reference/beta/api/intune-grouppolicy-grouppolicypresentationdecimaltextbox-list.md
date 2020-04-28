---
title: Список ГраупполиципресентатиондеЦималтекстбоксес
description: Список свойств и связей объектов ГраупполиципресентатиондеЦималтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e847e6a1b631a3897d2d773867fe69fb3f262312
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424434"
---
# <a name="list-grouppolicypresentationdecimaltextboxes"></a><span data-ttu-id="3de16-103">Список ГраупполиципресентатиондеЦималтекстбоксес</span><span class="sxs-lookup"><span data-stu-id="3de16-103">List groupPolicyPresentationDecimalTextBoxes</span></span>

<span data-ttu-id="3de16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3de16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3de16-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3de16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3de16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de16-107">Список свойств и связей объектов [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="3de16-107">List properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3de16-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3de16-108">Prerequisites</span></span>
<span data-ttu-id="3de16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de16-111">Permission type</span></span>|<span data-ttu-id="3de16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3de16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3de16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3de16-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3de16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de16-116">Not supported.</span></span>|
|<span data-ttu-id="3de16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3de16-117">Application</span></span>|<span data-ttu-id="3de16-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3de16-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3de16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="3de16-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3de16-120">Request headers</span></span>
|<span data-ttu-id="3de16-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3de16-121">Header</span></span>|<span data-ttu-id="3de16-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3de16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3de16-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de16-123">Authorization</span></span>|<span data-ttu-id="3de16-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3de16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3de16-125">Accept</span></span>|<span data-ttu-id="3de16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3de16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de16-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3de16-127">Request body</span></span>
<span data-ttu-id="3de16-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3de16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3de16-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3de16-129">Response</span></span>
<span data-ttu-id="3de16-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3de16-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de16-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3de16-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de16-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3de16-132">Request</span></span>
<span data-ttu-id="3de16-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3de16-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="3de16-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de16-134">Response</span></span>
<span data-ttu-id="3de16-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3de16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
      "label": "Label value",
      "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
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



