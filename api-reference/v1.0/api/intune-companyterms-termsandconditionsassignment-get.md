---
title: Получение объекта termsAndConditionsAssignment
description: Чтение свойств и связей объекта termsAndConditionsAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f84cb1b9bf1e6d1968ed029008ecd10bf54dd5b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515415"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="3e040-103">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="3e040-103">Get termsAndConditionsAssignment</span></span>

<span data-ttu-id="3e040-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e040-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e040-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e040-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e040-106">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3e040-106">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e040-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e040-107">Prerequisites</span></span>
<span data-ttu-id="3e040-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e040-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e040-110">Permission type</span></span>|<span data-ttu-id="3e040-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e040-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e040-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e040-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e040-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e040-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3e040-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e040-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e040-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e040-115">Not supported.</span></span>|
|<span data-ttu-id="3e040-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e040-116">Application</span></span>|<span data-ttu-id="3e040-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e040-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e040-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e040-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e040-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e040-119">Optional query parameters</span></span>
<span data-ttu-id="3e040-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e040-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e040-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e040-121">Request headers</span></span>
|<span data-ttu-id="3e040-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e040-122">Header</span></span>|<span data-ttu-id="3e040-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3e040-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e040-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e040-124">Authorization</span></span>|<span data-ttu-id="3e040-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e040-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e040-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3e040-126">Accept</span></span>|<span data-ttu-id="3e040-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3e040-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e040-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e040-128">Request body</span></span>
<span data-ttu-id="3e040-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e040-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e040-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e040-130">Response</span></span>
<span data-ttu-id="3e040-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e040-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e040-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3e040-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e040-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e040-133">Request</span></span>
<span data-ttu-id="3e040-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e040-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3e040-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e040-135">Response</span></span>
<span data-ttu-id="3e040-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e040-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




