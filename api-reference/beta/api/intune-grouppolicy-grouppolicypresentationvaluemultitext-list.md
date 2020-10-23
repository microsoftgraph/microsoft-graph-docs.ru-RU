---
title: Список Граупполиципресентатионвалуемултитекстс
description: Список свойств и связей объектов Граупполиципресентатионвалуемултитекст.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3ccbc8ea00a735a8fbd9146e26782cf6a7c53a3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698598"
---
# <a name="list-grouppolicypresentationvaluemultitexts"></a><span data-ttu-id="be0a3-103">Список Граупполиципресентатионвалуемултитекстс</span><span class="sxs-lookup"><span data-stu-id="be0a3-103">List groupPolicyPresentationValueMultiTexts</span></span>

<span data-ttu-id="be0a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be0a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be0a3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be0a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be0a3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be0a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be0a3-107">Список свойств и связей объектов [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="be0a3-107">List properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be0a3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be0a3-108">Prerequisites</span></span>
<span data-ttu-id="be0a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be0a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be0a3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be0a3-111">Permission type</span></span>|<span data-ttu-id="be0a3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be0a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be0a3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be0a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be0a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be0a3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="be0a3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be0a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be0a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be0a3-116">Not supported.</span></span>|
|<span data-ttu-id="be0a3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be0a3-117">Application</span></span>|<span data-ttu-id="be0a3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be0a3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be0a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be0a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="be0a3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be0a3-120">Request headers</span></span>
|<span data-ttu-id="be0a3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be0a3-121">Header</span></span>|<span data-ttu-id="be0a3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be0a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be0a3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be0a3-123">Authorization</span></span>|<span data-ttu-id="be0a3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be0a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be0a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be0a3-125">Accept</span></span>|<span data-ttu-id="be0a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be0a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be0a3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be0a3-127">Request body</span></span>
<span data-ttu-id="be0a3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be0a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be0a3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="be0a3-129">Response</span></span>
<span data-ttu-id="be0a3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be0a3-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be0a3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be0a3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="be0a3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be0a3-132">Request</span></span>
<span data-ttu-id="be0a3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be0a3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="be0a3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="be0a3-134">Response</span></span>
<span data-ttu-id="be0a3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be0a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





