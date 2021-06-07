---
title: Получение организации
description: Чтение свойств и связей объекта organization.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60520df5ae9de7f488870c271c6c69c96aa80273
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752506"
---
# <a name="get-organization"></a><span data-ttu-id="19afb-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="19afb-103">Get organization</span></span>

<span data-ttu-id="19afb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19afb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19afb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19afb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19afb-106">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="19afb-106">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19afb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19afb-107">Prerequisites</span></span>
<span data-ttu-id="19afb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19afb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19afb-110">Permission type</span></span>|<span data-ttu-id="19afb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19afb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19afb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19afb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19afb-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19afb-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="19afb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19afb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19afb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19afb-115">Not supported.</span></span>|
|<span data-ttu-id="19afb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="19afb-116">Application</span></span>|<span data-ttu-id="19afb-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19afb-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19afb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19afb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19afb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19afb-119">Optional query parameters</span></span>
<span data-ttu-id="19afb-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19afb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19afb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19afb-121">Request headers</span></span>
|<span data-ttu-id="19afb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19afb-122">Header</span></span>|<span data-ttu-id="19afb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="19afb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19afb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="19afb-124">Authorization</span></span>|<span data-ttu-id="19afb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19afb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19afb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="19afb-126">Accept</span></span>|<span data-ttu-id="19afb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19afb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19afb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19afb-128">Request body</span></span>
<span data-ttu-id="19afb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19afb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19afb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="19afb-130">Response</span></span>
<span data-ttu-id="19afb-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19afb-131">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19afb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="19afb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="19afb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="19afb-133">Request</span></span>
<span data-ttu-id="19afb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19afb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="19afb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="19afb-135">Response</span></span>
<span data-ttu-id="19afb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19afb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "value": {
    "@odata.type": "#microsoft.graph.organization",
    "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
    "mobileDeviceManagementAuthority": "intune"
  }
}
```




