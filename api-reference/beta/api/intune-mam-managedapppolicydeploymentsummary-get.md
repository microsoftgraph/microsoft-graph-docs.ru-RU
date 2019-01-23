---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9618178c05de75fcc099230103be40fb1aa08a8a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404752"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="6dc0a-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="6dc0a-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="6dc0a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6dc0a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6dc0a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc0a-107">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6dc0a-107">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc0a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6dc0a-108">Prerequisites</span></span>
<span data-ttu-id="6dc0a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6dc0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6dc0a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc0a-111">Permission type</span></span>|<span data-ttu-id="6dc0a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dc0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc0a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dc0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc0a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dc0a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6dc0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dc0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-116">Not supported.</span></span>|
|<span data-ttu-id="6dc0a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dc0a-117">Application</span></span>|<span data-ttu-id="6dc0a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc0a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dc0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dc0a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dc0a-120">Optional query parameters</span></span>
<span data-ttu-id="6dc0a-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dc0a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dc0a-122">Request headers</span></span>
|<span data-ttu-id="6dc0a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6dc0a-123">Header</span></span>|<span data-ttu-id="6dc0a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6dc0a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc0a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dc0a-125">Authorization</span></span>|<span data-ttu-id="6dc0a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6dc0a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc0a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6dc0a-127">Accept</span></span>|<span data-ttu-id="6dc0a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc0a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc0a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dc0a-129">Request body</span></span>
<span data-ttu-id="6dc0a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dc0a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc0a-131">Response</span></span>
<span data-ttu-id="6dc0a-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-132">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc0a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6dc0a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc0a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dc0a-134">Request</span></span>
<span data-ttu-id="6dc0a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="6dc0a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc0a-136">Response</span></span>
<span data-ttu-id="6dc0a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6dc0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
    "version": "Version value"
  }
}
```




