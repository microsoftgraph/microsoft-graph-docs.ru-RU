---
title: Получение организации
description: Чтение свойств и связей объекта organization.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 534dc20db95555fde23908b5d073a3846805896a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978600"
---
# <a name="get-organization"></a><span data-ttu-id="51be9-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="51be9-103">Get organization</span></span>

> <span data-ttu-id="51be9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51be9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51be9-105">Чтение свойств и связей объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="51be9-105">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51be9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51be9-106">Prerequisites</span></span>
<span data-ttu-id="51be9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51be9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51be9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51be9-109">Permission type</span></span>|<span data-ttu-id="51be9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51be9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51be9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51be9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51be9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="51be9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="51be9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51be9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51be9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51be9-114">Not supported.</span></span>|
|<span data-ttu-id="51be9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51be9-115">Application</span></span>|<span data-ttu-id="51be9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51be9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51be9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51be9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51be9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51be9-118">Optional query parameters</span></span>
<span data-ttu-id="51be9-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51be9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51be9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51be9-120">Request headers</span></span>
|<span data-ttu-id="51be9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51be9-121">Header</span></span>|<span data-ttu-id="51be9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51be9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51be9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51be9-123">Authorization</span></span>|<span data-ttu-id="51be9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51be9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51be9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51be9-125">Accept</span></span>|<span data-ttu-id="51be9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51be9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51be9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51be9-127">Request body</span></span>
<span data-ttu-id="51be9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51be9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51be9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51be9-129">Response</span></span>
<span data-ttu-id="51be9-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/intune-onboarding-organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51be9-130">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51be9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51be9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="51be9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51be9-132">Request</span></span>
<span data-ttu-id="51be9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51be9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="51be9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="51be9-134">Response</span></span>
<span data-ttu-id="51be9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51be9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



