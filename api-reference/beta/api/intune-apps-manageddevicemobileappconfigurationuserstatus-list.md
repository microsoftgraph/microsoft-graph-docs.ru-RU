---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a84dbee45b36c176853a638454f5829467b71da0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935383"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="183ec-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="183ec-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="183ec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="183ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="183ec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="183ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="183ec-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="183ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="183ec-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="183ec-107">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="183ec-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="183ec-108">Prerequisites</span></span>
<span data-ttu-id="183ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="183ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="183ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="183ec-111">Permission type</span></span>|<span data-ttu-id="183ec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="183ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="183ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="183ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="183ec-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="183ec-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="183ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="183ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="183ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="183ec-116">Not supported.</span></span>|
|<span data-ttu-id="183ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="183ec-117">Application</span></span>|<span data-ttu-id="183ec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="183ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="183ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="183ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="183ec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="183ec-120">Request headers</span></span>
|<span data-ttu-id="183ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="183ec-121">Header</span></span>|<span data-ttu-id="183ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="183ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="183ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="183ec-123">Authorization</span></span>|<span data-ttu-id="183ec-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="183ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="183ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="183ec-125">Accept</span></span>|<span data-ttu-id="183ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="183ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="183ec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="183ec-127">Request body</span></span>
<span data-ttu-id="183ec-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="183ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="183ec-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="183ec-129">Response</span></span>
<span data-ttu-id="183ec-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="183ec-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="183ec-131">Пример</span><span class="sxs-lookup"><span data-stu-id="183ec-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="183ec-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="183ec-132">Request</span></span>
<span data-ttu-id="183ec-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="183ec-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="183ec-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="183ec-134">Response</span></span>
<span data-ttu-id="183ec-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="183ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





