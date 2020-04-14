---
title: Получение Мобилеаппинтентандстате
description: Чтение свойств и связей объекта Мобилеаппинтентандстате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 289969faf158d11181a49ea33c9823c6065cb091
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455399"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="c2154-103">Получение Мобилеаппинтентандстате</span><span class="sxs-lookup"><span data-stu-id="c2154-103">Get mobileAppIntentAndState</span></span>

<span data-ttu-id="c2154-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2154-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2154-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2154-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2154-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2154-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2154-107">Чтение свойств и связей объекта [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c2154-107">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2154-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2154-108">Prerequisites</span></span>
<span data-ttu-id="c2154-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2154-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2154-111">Permission type</span></span>|<span data-ttu-id="c2154-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2154-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2154-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2154-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2154-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2154-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c2154-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2154-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2154-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2154-116">Not supported.</span></span>|
|<span data-ttu-id="c2154-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2154-117">Application</span></span>|<span data-ttu-id="c2154-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2154-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2154-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2154-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2154-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2154-120">Optional query parameters</span></span>
<span data-ttu-id="c2154-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2154-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2154-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2154-122">Request headers</span></span>
|<span data-ttu-id="c2154-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2154-123">Header</span></span>|<span data-ttu-id="c2154-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c2154-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2154-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2154-125">Authorization</span></span>|<span data-ttu-id="c2154-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2154-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2154-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c2154-127">Accept</span></span>|<span data-ttu-id="c2154-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2154-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2154-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2154-129">Request body</span></span>
<span data-ttu-id="c2154-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2154-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2154-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2154-131">Response</span></span>
<span data-ttu-id="c2154-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мобилеаппинтентандстате](../resources/intune-troubleshooting-mobileappintentandstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2154-132">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2154-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2154-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2154-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2154-134">Request</span></span>
<span data-ttu-id="c2154-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2154-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="c2154-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2154-136">Response</span></span>
<span data-ttu-id="c2154-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2154-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



