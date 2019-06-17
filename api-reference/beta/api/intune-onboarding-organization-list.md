---
title: Список организаций
description: Список свойств и связей объектов organization.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d49120c67c520ff17dd9cb7aeabd9e60045c388
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980700"
---
# <a name="list-organizations"></a><span data-ttu-id="55174-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="55174-103">List organizations</span></span>

> <span data-ttu-id="55174-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55174-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55174-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55174-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55174-106">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="55174-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55174-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55174-107">Prerequisites</span></span>
<span data-ttu-id="55174-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55174-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55174-110">Permission type</span></span>|<span data-ttu-id="55174-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55174-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55174-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55174-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55174-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="55174-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="55174-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55174-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55174-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55174-115">Not supported.</span></span>|
|<span data-ttu-id="55174-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55174-116">Application</span></span>|<span data-ttu-id="55174-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55174-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55174-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55174-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="55174-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55174-119">Request headers</span></span>
|<span data-ttu-id="55174-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55174-120">Header</span></span>|<span data-ttu-id="55174-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55174-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55174-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55174-122">Authorization</span></span>|<span data-ttu-id="55174-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55174-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55174-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55174-124">Accept</span></span>|<span data-ttu-id="55174-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55174-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55174-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55174-126">Request body</span></span>
<span data-ttu-id="55174-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55174-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55174-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="55174-128">Response</span></span>
<span data-ttu-id="55174-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="55174-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55174-130">Пример</span><span class="sxs-lookup"><span data-stu-id="55174-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="55174-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="55174-131">Request</span></span>
<span data-ttu-id="55174-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55174-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization
```

### <a name="response"></a><span data-ttu-id="55174-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="55174-133">Response</span></span>
<span data-ttu-id="55174-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55174-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune",
      "certificateConnectorSetting": {
        "@odata.type": "microsoft.graph.certificateConnectorSetting",
        "status": 6,
        "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
        "enrollmentError": "Enrollment Error value",
        "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
        "connectorVersion": "Connector Version value",
        "lastUploadVersion": 1
      }
    }
  ]
}
```





