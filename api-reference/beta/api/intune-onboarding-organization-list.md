---
title: Список организаций
description: Список свойств и связей объектов organization.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 067489dad7e08053cd4e6004f1e8b20fca479853
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807758"
---
# <a name="list-organizations"></a><span data-ttu-id="5c8f7-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="5c8f7-103">List organizations</span></span>

> <span data-ttu-id="5c8f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c8f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c8f7-106">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="5c8f7-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c8f7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c8f7-107">Prerequisites</span></span>
<span data-ttu-id="5c8f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c8f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8f7-110">Permission type</span></span>|<span data-ttu-id="5c8f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c8f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c8f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c8f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c8f7-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c8f7-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5c8f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c8f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c8f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-115">Not supported.</span></span>|
|<span data-ttu-id="5c8f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c8f7-116">Application</span></span>|<span data-ttu-id="5c8f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c8f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c8f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="5c8f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c8f7-119">Request headers</span></span>
|<span data-ttu-id="5c8f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c8f7-120">Header</span></span>|<span data-ttu-id="5c8f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c8f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c8f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c8f7-122">Authorization</span></span>|<span data-ttu-id="5c8f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c8f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c8f7-124">Accept</span></span>|<span data-ttu-id="5c8f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c8f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c8f7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c8f7-126">Request body</span></span>
<span data-ttu-id="5c8f7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c8f7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c8f7-128">Response</span></span>
<span data-ttu-id="5c8f7-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c8f7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5c8f7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c8f7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c8f7-131">Request</span></span>
<span data-ttu-id="5c8f7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization
```

### <a name="response"></a><span data-ttu-id="5c8f7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c8f7-133">Response</span></span>
<span data-ttu-id="5c8f7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c8f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





