---
title: Список Граупполиципресентатионвалуетекстс
description: Список свойств и связей объектов Граупполиципресентатионвалуетекст.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d62922702d8e19b4b7f2f968f39360f0e38f04d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530538"
---
# <a name="list-grouppolicypresentationvaluetexts"></a><span data-ttu-id="21bdc-103">Список Граупполиципресентатионвалуетекстс</span><span class="sxs-lookup"><span data-stu-id="21bdc-103">List groupPolicyPresentationValueTexts</span></span>

> <span data-ttu-id="21bdc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bdc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bdc-106">Список свойств и связей объектов [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="21bdc-106">List properties and relationships of the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21bdc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21bdc-107">Prerequisites</span></span>
<span data-ttu-id="21bdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21bdc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21bdc-110">Permission type</span></span>|<span data-ttu-id="21bdc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21bdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21bdc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21bdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21bdc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="21bdc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="21bdc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21bdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21bdc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bdc-115">Not supported.</span></span>|
|<span data-ttu-id="21bdc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21bdc-116">Application</span></span>|<span data-ttu-id="21bdc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bdc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21bdc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21bdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="21bdc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21bdc-119">Request headers</span></span>
|<span data-ttu-id="21bdc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21bdc-120">Header</span></span>|<span data-ttu-id="21bdc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="21bdc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21bdc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21bdc-122">Authorization</span></span>|<span data-ttu-id="21bdc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21bdc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21bdc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="21bdc-124">Accept</span></span>|<span data-ttu-id="21bdc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21bdc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21bdc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21bdc-126">Request body</span></span>
<span data-ttu-id="21bdc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21bdc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21bdc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="21bdc-128">Response</span></span>
<span data-ttu-id="21bdc-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21bdc-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21bdc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="21bdc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="21bdc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="21bdc-131">Request</span></span>
<span data-ttu-id="21bdc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21bdc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="21bdc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="21bdc-133">Response</span></span>
<span data-ttu-id="21bdc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21bdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "a3883444-3444-a388-4434-88a3443488a3",
      "value": "Value value"
    }
  ]
}
```





