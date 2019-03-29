---
title: Получение организации
description: Чтение свойств и связей объекта organization.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7eef2cf09e04728206cae427646e1fbc3da15a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971124"
---
# <a name="get-organization"></a><span data-ttu-id="3fa32-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="3fa32-103">Get organization</span></span>

> <span data-ttu-id="3fa32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fa32-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fa32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fa32-106">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="3fa32-106">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fa32-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3fa32-107">Prerequisites</span></span>
<span data-ttu-id="3fa32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa32-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa32-110">Permission type</span></span>|<span data-ttu-id="3fa32-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fa32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fa32-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa32-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fa32-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3fa32-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fa32-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa32-115">Not supported.</span></span>|
|<span data-ttu-id="3fa32-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fa32-116">Application</span></span>|<span data-ttu-id="3fa32-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa32-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa32-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fa32-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3fa32-119">Optional query parameters</span></span>
<span data-ttu-id="3fa32-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3fa32-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fa32-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fa32-121">Request headers</span></span>
|<span data-ttu-id="3fa32-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fa32-122">Header</span></span>|<span data-ttu-id="3fa32-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3fa32-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fa32-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fa32-124">Authorization</span></span>|<span data-ttu-id="3fa32-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa32-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fa32-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3fa32-126">Accept</span></span>|<span data-ttu-id="3fa32-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3fa32-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa32-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fa32-128">Request body</span></span>
<span data-ttu-id="3fa32-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fa32-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fa32-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa32-130">Response</span></span>
<span data-ttu-id="3fa32-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fa32-131">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa32-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa32-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa32-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa32-133">Request</span></span>
<span data-ttu-id="3fa32-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fa32-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="3fa32-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa32-135">Response</span></span>
<span data-ttu-id="3fa32-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fa32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




