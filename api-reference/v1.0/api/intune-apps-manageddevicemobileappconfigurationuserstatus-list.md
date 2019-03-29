---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31471db6eea629d09d1a458bafa9e9798a2df2a9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956816"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="b001d-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="b001d-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="b001d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b001d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b001d-105">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b001d-105">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b001d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b001d-106">Prerequisites</span></span>
<span data-ttu-id="b001d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b001d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b001d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b001d-109">Permission type</span></span>|<span data-ttu-id="b001d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b001d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b001d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b001d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b001d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b001d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b001d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b001d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b001d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b001d-114">Not supported.</span></span>|
|<span data-ttu-id="b001d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b001d-115">Application</span></span>|<span data-ttu-id="b001d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b001d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b001d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b001d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b001d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b001d-118">Request headers</span></span>
|<span data-ttu-id="b001d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b001d-119">Header</span></span>|<span data-ttu-id="b001d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b001d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b001d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b001d-121">Authorization</span></span>|<span data-ttu-id="b001d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b001d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b001d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b001d-123">Accept</span></span>|<span data-ttu-id="b001d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b001d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b001d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b001d-125">Request body</span></span>
<span data-ttu-id="b001d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b001d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b001d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b001d-127">Response</span></span>
<span data-ttu-id="b001d-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b001d-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b001d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b001d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b001d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b001d-130">Request</span></span>
<span data-ttu-id="b001d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b001d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="b001d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b001d-132">Response</span></span>
<span data-ttu-id="b001d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b001d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



