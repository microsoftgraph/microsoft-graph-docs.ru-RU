---
title: Получение Девицеманажементексчанжеонпремисесполици
description: Чтение свойств и связей объекта Девицеманажементексчанжеонпремисесполици.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c81bbfb81d59e931f700b9a46999548a7eca9a37
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802897"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="ab022-103">Получение Девицеманажементексчанжеонпремисесполици</span><span class="sxs-lookup"><span data-stu-id="ab022-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="ab022-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab022-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab022-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab022-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab022-106">Чтение свойств и связей объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab022-106">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab022-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab022-107">Prerequisites</span></span>
<span data-ttu-id="ab022-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab022-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab022-110">Permission type</span></span>|<span data-ttu-id="ab022-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab022-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab022-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab022-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab022-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab022-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ab022-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab022-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab022-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab022-115">Not supported.</span></span>|
|<span data-ttu-id="ab022-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab022-116">Application</span></span>|<span data-ttu-id="ab022-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab022-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab022-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab022-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab022-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab022-119">Optional query parameters</span></span>
<span data-ttu-id="ab022-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ab022-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab022-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab022-121">Request headers</span></span>
|<span data-ttu-id="ab022-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab022-122">Header</span></span>|<span data-ttu-id="ab022-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ab022-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab022-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab022-124">Authorization</span></span>|<span data-ttu-id="ab022-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab022-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab022-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ab022-126">Accept</span></span>|<span data-ttu-id="ab022-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ab022-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab022-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab022-128">Request body</span></span>
<span data-ttu-id="ab022-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab022-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab022-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab022-130">Response</span></span>
<span data-ttu-id="ab022-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab022-131">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab022-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ab022-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab022-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab022-133">Request</span></span>
<span data-ttu-id="ab022-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab022-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="ab022-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab022-135">Response</span></span>
<span data-ttu-id="ab022-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "16e76336-6336-16e7-3663-e7163663e716",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "allow",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "model"
        },
        "accessLevel": "allow"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      }
    ]
  }
}
```




