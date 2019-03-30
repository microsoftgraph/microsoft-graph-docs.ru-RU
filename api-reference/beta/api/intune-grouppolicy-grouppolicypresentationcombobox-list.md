---
title: Список Граупполиципресентатионкомбобоксес
description: Список свойств и связей объектов Граупполиципресентатионкомбобокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8af70fc0026a5cbc30f9c93d7de683cf078dbdc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964509"
---
# <a name="list-grouppolicypresentationcomboboxes"></a><span data-ttu-id="ecffc-103">Список Граупполиципресентатионкомбобоксес</span><span class="sxs-lookup"><span data-stu-id="ecffc-103">List groupPolicyPresentationComboBoxes</span></span>

> <span data-ttu-id="ecffc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecffc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecffc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ecffc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecffc-106">Список свойств и связей объектов [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .</span><span class="sxs-lookup"><span data-stu-id="ecffc-106">List properties and relationships of the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecffc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ecffc-107">Prerequisites</span></span>
<span data-ttu-id="ecffc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecffc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecffc-110">Permission type</span></span>|<span data-ttu-id="ecffc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecffc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecffc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecffc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecffc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecffc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ecffc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecffc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecffc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecffc-115">Not supported.</span></span>|
|<span data-ttu-id="ecffc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecffc-116">Application</span></span>|<span data-ttu-id="ecffc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecffc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecffc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecffc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="ecffc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecffc-119">Request headers</span></span>
|<span data-ttu-id="ecffc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ecffc-120">Header</span></span>|<span data-ttu-id="ecffc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ecffc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecffc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecffc-122">Authorization</span></span>|<span data-ttu-id="ecffc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecffc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecffc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ecffc-124">Accept</span></span>|<span data-ttu-id="ecffc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecffc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecffc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecffc-126">Request body</span></span>
<span data-ttu-id="ecffc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecffc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecffc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecffc-128">Response</span></span>
<span data-ttu-id="ecffc-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ecffc-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecffc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ecffc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecffc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecffc-131">Request</span></span>
<span data-ttu-id="ecffc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecffc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="ecffc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecffc-133">Response</span></span>
<span data-ttu-id="ecffc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecffc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "value": [
    {
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
  ]
}
```




