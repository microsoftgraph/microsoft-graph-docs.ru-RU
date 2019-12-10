---
title: Список Мобилеаппполицисетитемс
description: Список свойств и связей объектов Мобилеаппполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5f68819fb406fd234d769fd5ede1601284f1dba
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940996"
---
# <a name="list-mobileapppolicysetitems"></a><span data-ttu-id="55ccf-103">Список Мобилеаппполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="55ccf-103">List mobileAppPolicySetItems</span></span>

> <span data-ttu-id="55ccf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ccf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55ccf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55ccf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55ccf-106">Список свойств и связей объектов [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="55ccf-106">List properties and relationships of the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55ccf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55ccf-107">Prerequisites</span></span>
<span data-ttu-id="55ccf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55ccf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55ccf-110">Permission type</span></span>|<span data-ttu-id="55ccf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55ccf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55ccf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55ccf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55ccf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55ccf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55ccf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55ccf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55ccf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ccf-115">Not supported.</span></span>|
|<span data-ttu-id="55ccf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55ccf-116">Application</span></span>|<span data-ttu-id="55ccf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55ccf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55ccf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55ccf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="55ccf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55ccf-119">Request headers</span></span>
|<span data-ttu-id="55ccf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55ccf-120">Header</span></span>|<span data-ttu-id="55ccf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55ccf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55ccf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55ccf-122">Authorization</span></span>|<span data-ttu-id="55ccf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55ccf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55ccf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55ccf-124">Accept</span></span>|<span data-ttu-id="55ccf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55ccf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55ccf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55ccf-126">Request body</span></span>
<span data-ttu-id="55ccf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55ccf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55ccf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="55ccf-128">Response</span></span>
<span data-ttu-id="55ccf-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55ccf-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55ccf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="55ccf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="55ccf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="55ccf-131">Request</span></span>
<span data-ttu-id="55ccf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55ccf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="55ccf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="55ccf-133">Response</span></span>
<span data-ttu-id="55ccf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55ccf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
      "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "intent": "required",
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```





