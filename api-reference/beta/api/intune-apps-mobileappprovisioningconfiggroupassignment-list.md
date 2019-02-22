---
title: Список Мобилеапппровисионингконфигграупассигнментс
description: Список свойств и связей объектов К mobileappprovisioningconfiggroupassignment..
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb880a48e28b5d9e131d2a62c59249e168657745
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140336"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="1109c-103">Список Мобилеапппровисионингконфигграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="1109c-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="1109c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1109c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1109c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1109c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1109c-106">Список свойств и связей объектов [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1109c-106">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1109c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1109c-107">Prerequisites</span></span>
<span data-ttu-id="1109c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1109c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1109c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1109c-110">Permission type</span></span>|<span data-ttu-id="1109c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1109c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1109c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1109c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1109c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1109c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1109c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1109c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1109c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1109c-115">Not supported.</span></span>|
|<span data-ttu-id="1109c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1109c-116">Application</span></span>|<span data-ttu-id="1109c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1109c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1109c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1109c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="1109c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1109c-119">Request headers</span></span>
|<span data-ttu-id="1109c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1109c-120">Header</span></span>|<span data-ttu-id="1109c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1109c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1109c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1109c-122">Authorization</span></span>|<span data-ttu-id="1109c-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1109c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1109c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1109c-124">Accept</span></span>|<span data-ttu-id="1109c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1109c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1109c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1109c-126">Request body</span></span>
<span data-ttu-id="1109c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1109c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1109c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1109c-128">Response</span></span>
<span data-ttu-id="1109c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1109c-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1109c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1109c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1109c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1109c-131">Request</span></span>
<span data-ttu-id="1109c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1109c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="1109c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1109c-133">Response</span></span>
<span data-ttu-id="1109c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1109c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




