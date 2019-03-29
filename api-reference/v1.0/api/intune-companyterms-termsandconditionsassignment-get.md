---
title: Получение объекта termsAndConditionsAssignment
description: Чтение свойств и связей объекта termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b11016cb45ef3db70d9779e1bbd0d3f2bb1a8857
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970312"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="3e37c-103">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="3e37c-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="3e37c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e37c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e37c-105">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3e37c-105">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e37c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e37c-106">Prerequisites</span></span>
<span data-ttu-id="3e37c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e37c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e37c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e37c-109">Permission type</span></span>|<span data-ttu-id="3e37c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e37c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e37c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e37c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e37c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e37c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3e37c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e37c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e37c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e37c-114">Not supported.</span></span>|
|<span data-ttu-id="3e37c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e37c-115">Application</span></span>|<span data-ttu-id="3e37c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e37c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e37c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e37c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e37c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e37c-118">Optional query parameters</span></span>
<span data-ttu-id="3e37c-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e37c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e37c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e37c-120">Request headers</span></span>
|<span data-ttu-id="3e37c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e37c-121">Header</span></span>|<span data-ttu-id="3e37c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e37c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e37c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e37c-123">Authorization</span></span>|<span data-ttu-id="3e37c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e37c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e37c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e37c-125">Accept</span></span>|<span data-ttu-id="3e37c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e37c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e37c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e37c-127">Request body</span></span>
<span data-ttu-id="3e37c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e37c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e37c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e37c-129">Response</span></span>
<span data-ttu-id="3e37c-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e37c-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e37c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e37c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e37c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e37c-132">Request</span></span>
<span data-ttu-id="3e37c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e37c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3e37c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e37c-134">Response</span></span>
<span data-ttu-id="3e37c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e37c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



