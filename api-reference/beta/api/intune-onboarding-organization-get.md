---
title: Получение организации
description: Чтение свойств и связей объекта organization.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cc83a51fc9829b4c396409dbdd0e8baa71c3ba5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410289"
---
# <a name="get-organization"></a><span data-ttu-id="c7094-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="c7094-103">Get organization</span></span>

> <span data-ttu-id="c7094-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7094-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7094-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7094-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7094-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7094-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7094-107">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="c7094-107">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7094-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c7094-108">Prerequisites</span></span>
<span data-ttu-id="c7094-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7094-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7094-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7094-111">Permission type</span></span>|<span data-ttu-id="c7094-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7094-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7094-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7094-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7094-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7094-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c7094-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7094-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7094-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7094-116">Not supported.</span></span>|
|<span data-ttu-id="c7094-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7094-117">Application</span></span>|<span data-ttu-id="c7094-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7094-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7094-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7094-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7094-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7094-120">Optional query parameters</span></span>
<span data-ttu-id="c7094-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7094-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7094-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7094-122">Request headers</span></span>
|<span data-ttu-id="c7094-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7094-123">Header</span></span>|<span data-ttu-id="c7094-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c7094-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7094-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7094-125">Authorization</span></span>|<span data-ttu-id="c7094-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7094-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7094-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c7094-127">Accept</span></span>|<span data-ttu-id="c7094-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7094-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7094-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7094-129">Request body</span></span>
<span data-ttu-id="c7094-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7094-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7094-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7094-131">Response</span></span>
<span data-ttu-id="c7094-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7094-132">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7094-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c7094-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7094-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7094-134">Request</span></span>
<span data-ttu-id="c7094-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7094-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="c7094-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7094-136">Response</span></span>
<span data-ttu-id="c7094-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7094-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




