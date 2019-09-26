---
title: Получение организации
description: Чтение свойств и связей объекта organization.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17ba91765225e22c04adf7f87ffbf9893b075531
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190371"
---
# <a name="get-organization"></a><span data-ttu-id="57742-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="57742-103">Get organization</span></span>

> <span data-ttu-id="57742-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57742-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57742-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57742-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57742-106">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="57742-106">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57742-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="57742-107">Prerequisites</span></span>
<span data-ttu-id="57742-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57742-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57742-110">Permission type</span></span>|<span data-ttu-id="57742-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57742-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57742-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57742-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57742-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="57742-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="57742-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57742-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57742-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57742-115">Not supported.</span></span>|
|<span data-ttu-id="57742-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57742-116">Application</span></span>|<span data-ttu-id="57742-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="57742-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57742-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57742-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57742-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57742-119">Optional query parameters</span></span>
<span data-ttu-id="57742-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57742-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57742-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57742-121">Request headers</span></span>
|<span data-ttu-id="57742-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57742-122">Header</span></span>|<span data-ttu-id="57742-123">Значение</span><span class="sxs-lookup"><span data-stu-id="57742-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57742-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57742-124">Authorization</span></span>|<span data-ttu-id="57742-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57742-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57742-126">Accept</span><span class="sxs-lookup"><span data-stu-id="57742-126">Accept</span></span>|<span data-ttu-id="57742-127">application/json</span><span class="sxs-lookup"><span data-stu-id="57742-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57742-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57742-128">Request body</span></span>
<span data-ttu-id="57742-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57742-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57742-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="57742-130">Response</span></span>
<span data-ttu-id="57742-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57742-131">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57742-132">Пример</span><span class="sxs-lookup"><span data-stu-id="57742-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="57742-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="57742-133">Request</span></span>
<span data-ttu-id="57742-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57742-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="57742-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="57742-135">Response</span></span>
<span data-ttu-id="57742-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57742-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




