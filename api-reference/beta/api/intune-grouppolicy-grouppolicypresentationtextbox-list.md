---
title: Список Граупполиципресентатионтекстбоксес
description: Список свойств и связей объектов Граупполиципресентатионтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86eede6f244828e87b2794ebd2886aa7398a3b83
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408506"
---
# <a name="list-grouppolicypresentationtextboxes"></a><span data-ttu-id="c5265-103">Список Граупполиципресентатионтекстбоксес</span><span class="sxs-lookup"><span data-stu-id="c5265-103">List groupPolicyPresentationTextBoxes</span></span>

<span data-ttu-id="c5265-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5265-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5265-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5265-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5265-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5265-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5265-107">Список свойств и связей объектов [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="c5265-107">List properties and relationships of the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5265-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5265-108">Prerequisites</span></span>
<span data-ttu-id="c5265-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5265-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5265-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5265-111">Permission type</span></span>|<span data-ttu-id="c5265-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5265-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5265-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5265-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5265-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5265-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5265-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5265-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5265-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5265-116">Not supported.</span></span>|
|<span data-ttu-id="c5265-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5265-117">Application</span></span>|<span data-ttu-id="c5265-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5265-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5265-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5265-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="c5265-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5265-120">Request headers</span></span>
|<span data-ttu-id="c5265-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5265-121">Header</span></span>|<span data-ttu-id="c5265-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5265-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5265-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5265-123">Authorization</span></span>|<span data-ttu-id="c5265-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5265-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5265-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5265-125">Accept</span></span>|<span data-ttu-id="c5265-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5265-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5265-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5265-127">Request body</span></span>
<span data-ttu-id="c5265-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5265-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5265-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5265-129">Response</span></span>
<span data-ttu-id="c5265-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5265-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5265-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c5265-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5265-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5265-132">Request</span></span>
<span data-ttu-id="c5265-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5265-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="c5265-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5265-134">Response</span></span>
<span data-ttu-id="c5265-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5265-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
      "label": "Label value",
      "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultValue": "Default Value value",
      "required": true,
      "maxLength": 9
    }
  ]
}
```



