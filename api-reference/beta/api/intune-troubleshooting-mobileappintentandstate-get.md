---
title: Get mobileAppIntentAndState
description: Чтение свойств и связей объекта mobileAppIntentAndState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d71c3ab2615285594d1025f4c799b16bc584309d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151839"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="97e39-103">Get mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="97e39-103">Get mobileAppIntentAndState</span></span>

<span data-ttu-id="97e39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97e39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97e39-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97e39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97e39-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97e39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97e39-107">Чтение свойств и связей объекта [mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)</span><span class="sxs-lookup"><span data-stu-id="97e39-107">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97e39-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97e39-108">Prerequisites</span></span>
<span data-ttu-id="97e39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97e39-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97e39-111">Permission type</span></span>|<span data-ttu-id="97e39-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97e39-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97e39-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97e39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97e39-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97e39-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="97e39-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97e39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97e39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97e39-116">Not supported.</span></span>|
|<span data-ttu-id="97e39-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="97e39-117">Application</span></span>|<span data-ttu-id="97e39-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97e39-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97e39-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97e39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97e39-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="97e39-120">Optional query parameters</span></span>
<span data-ttu-id="97e39-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97e39-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97e39-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97e39-122">Request headers</span></span>
|<span data-ttu-id="97e39-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97e39-123">Header</span></span>|<span data-ttu-id="97e39-124">Значение</span><span class="sxs-lookup"><span data-stu-id="97e39-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97e39-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="97e39-125">Authorization</span></span>|<span data-ttu-id="97e39-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97e39-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97e39-127">Accept</span><span class="sxs-lookup"><span data-stu-id="97e39-127">Accept</span></span>|<span data-ttu-id="97e39-128">application/json</span><span class="sxs-lookup"><span data-stu-id="97e39-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97e39-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97e39-129">Request body</span></span>
<span data-ttu-id="97e39-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97e39-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97e39-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="97e39-131">Response</span></span>
<span data-ttu-id="97e39-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="97e39-132">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97e39-133">Пример</span><span class="sxs-lookup"><span data-stu-id="97e39-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="97e39-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="97e39-134">Request</span></span>
<span data-ttu-id="97e39-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97e39-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="97e39-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="97e39-136">Response</span></span>
<span data-ttu-id="97e39-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97e39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 943

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
    "id": "45a775d6-75d6-45a7-d675-a745d675a745",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "mobileAppList": [
      {
        "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
        "applicationId": "Application Id value",
        "displayName": "Display Name value",
        "mobileAppIntent": "notAvailable",
        "displayVersion": "Display Version value",
        "installState": "failed",
        "supportedDeviceTypes": [
          {
            "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
            "type": "windowsRT",
            "minimumOperatingSystemVersion": "Minimum Operating System Version value",
            "maximumOperatingSystemVersion": "Maximum Operating System Version value"
          }
        ]
      }
    ]
  }
}
```




