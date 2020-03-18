---
title: Получение Мобилеаппинтентандстате
description: Чтение свойств и связей объекта Мобилеаппинтентандстате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef9786aefdf7de093dbcf05472c55e7d19324a45
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800111"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="4d140-103">Получение Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="4d140-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="4d140-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d140-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d140-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d140-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d140-106">Чтение свойств и связей объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="4d140-106">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d140-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d140-107">Prerequisites</span></span>
<span data-ttu-id="4d140-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d140-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d140-110">Permission type</span></span>|<span data-ttu-id="4d140-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d140-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d140-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d140-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d140-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d140-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4d140-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d140-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d140-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d140-115">Not supported.</span></span>|
|<span data-ttu-id="4d140-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4d140-116">Application</span></span>|<span data-ttu-id="4d140-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d140-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d140-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d140-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d140-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d140-119">Optional query parameters</span></span>
<span data-ttu-id="4d140-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d140-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d140-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d140-121">Request headers</span></span>
|<span data-ttu-id="4d140-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d140-122">Header</span></span>|<span data-ttu-id="4d140-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4d140-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d140-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d140-124">Authorization</span></span>|<span data-ttu-id="4d140-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d140-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d140-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4d140-126">Accept</span></span>|<span data-ttu-id="4d140-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4d140-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d140-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d140-128">Request body</span></span>
<span data-ttu-id="4d140-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d140-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d140-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d140-130">Response</span></span>
<span data-ttu-id="4d140-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d140-131">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d140-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4d140-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d140-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d140-133">Request</span></span>
<span data-ttu-id="4d140-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d140-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="4d140-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d140-135">Response</span></span>
<span data-ttu-id="4d140-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




