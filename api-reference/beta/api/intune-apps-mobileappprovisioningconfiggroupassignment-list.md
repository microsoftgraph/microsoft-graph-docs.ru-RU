---
title: Список Мобилеапппровисионингконфигграупассигнментс
description: Список свойств и связей объектов К mobileappprovisioningconfiggroupassignment..
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5897dc00ed6e36c1bcbcfc615b0e6a416d21682a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336455"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="462eb-103">Список Мобилеапппровисионингконфигграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="462eb-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="462eb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="462eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="462eb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="462eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="462eb-106">Список свойств и связей объектов [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="462eb-106">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="462eb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="462eb-107">Prerequisites</span></span>
<span data-ttu-id="462eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="462eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="462eb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="462eb-110">Permission type</span></span>|<span data-ttu-id="462eb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="462eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="462eb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="462eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="462eb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="462eb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="462eb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="462eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="462eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="462eb-115">Not supported.</span></span>|
|<span data-ttu-id="462eb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="462eb-116">Application</span></span>|<span data-ttu-id="462eb-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="462eb-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="462eb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="462eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="462eb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="462eb-119">Request headers</span></span>
|<span data-ttu-id="462eb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="462eb-120">Header</span></span>|<span data-ttu-id="462eb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="462eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="462eb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="462eb-122">Authorization</span></span>|<span data-ttu-id="462eb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="462eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="462eb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="462eb-124">Accept</span></span>|<span data-ttu-id="462eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="462eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="462eb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="462eb-126">Request body</span></span>
<span data-ttu-id="462eb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="462eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="462eb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="462eb-128">Response</span></span>
<span data-ttu-id="462eb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="462eb-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="462eb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="462eb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="462eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="462eb-131">Request</span></span>
<span data-ttu-id="462eb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="462eb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="462eb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="462eb-133">Response</span></span>
<span data-ttu-id="462eb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="462eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ]
}
```






