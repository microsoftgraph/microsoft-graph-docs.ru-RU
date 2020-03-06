---
title: Получение организации
description: Чтение свойств и связей объекта organization.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a77b19c75ab7e5740973fd7a1feff8de2abf894a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512428"
---
# <a name="get-organization"></a><span data-ttu-id="9499f-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="9499f-103">Get organization</span></span>

<span data-ttu-id="9499f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9499f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9499f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9499f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9499f-106">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="9499f-106">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9499f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9499f-107">Prerequisites</span></span>
<span data-ttu-id="9499f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9499f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9499f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9499f-110">Permission type</span></span>|<span data-ttu-id="9499f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9499f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9499f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9499f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9499f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9499f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9499f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9499f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9499f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9499f-115">Not supported.</span></span>|
|<span data-ttu-id="9499f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9499f-116">Application</span></span>|<span data-ttu-id="9499f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9499f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9499f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9499f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9499f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9499f-119">Optional query parameters</span></span>
<span data-ttu-id="9499f-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9499f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9499f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9499f-121">Request headers</span></span>
|<span data-ttu-id="9499f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9499f-122">Header</span></span>|<span data-ttu-id="9499f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9499f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9499f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9499f-124">Authorization</span></span>|<span data-ttu-id="9499f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9499f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9499f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9499f-126">Accept</span></span>|<span data-ttu-id="9499f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9499f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9499f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9499f-128">Request body</span></span>
<span data-ttu-id="9499f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9499f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9499f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9499f-130">Response</span></span>
<span data-ttu-id="9499f-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9499f-131">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9499f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9499f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9499f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9499f-133">Request</span></span>
<span data-ttu-id="9499f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9499f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="9499f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9499f-135">Response</span></span>
<span data-ttu-id="9499f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9499f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




