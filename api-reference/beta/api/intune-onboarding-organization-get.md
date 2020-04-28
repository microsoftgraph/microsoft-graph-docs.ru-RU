---
title: Получение организации
description: Чтение свойств и связей объекта organization.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cfb8429f0aba8c17f3bc940a7e020be045f905df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377654"
---
# <a name="get-organization"></a><span data-ttu-id="d1e5e-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="d1e5e-103">Get organization</span></span>

<span data-ttu-id="d1e5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1e5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1e5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1e5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1e5e-107">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="d1e5e-107">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1e5e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1e5e-108">Prerequisites</span></span>
<span data-ttu-id="d1e5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e5e-111">Permission type</span></span>|<span data-ttu-id="d1e5e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1e5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1e5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1e5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1e5e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1e5e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d1e5e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1e5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1e5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-116">Not supported.</span></span>|
|<span data-ttu-id="d1e5e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1e5e-117">Application</span></span>|<span data-ttu-id="d1e5e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1e5e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1e5e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1e5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1e5e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1e5e-120">Optional query parameters</span></span>
<span data-ttu-id="d1e5e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1e5e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1e5e-122">Request headers</span></span>
|<span data-ttu-id="d1e5e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1e5e-123">Header</span></span>|<span data-ttu-id="d1e5e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d1e5e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1e5e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1e5e-125">Authorization</span></span>|<span data-ttu-id="d1e5e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1e5e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d1e5e-127">Accept</span></span>|<span data-ttu-id="d1e5e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d1e5e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1e5e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1e5e-129">Request body</span></span>
<span data-ttu-id="d1e5e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1e5e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1e5e-131">Response</span></span>
<span data-ttu-id="d1e5e-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-132">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1e5e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d1e5e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1e5e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1e5e-134">Request</span></span>
<span data-ttu-id="d1e5e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="d1e5e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e5e-136">Response</span></span>
<span data-ttu-id="d1e5e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 584

{
  "value": {
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
}
```



