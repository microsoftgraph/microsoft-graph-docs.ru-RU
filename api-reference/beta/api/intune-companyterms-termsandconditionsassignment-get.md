---
title: Получение объекта termsAndConditionsAssignment
description: Чтение свойств и связей объекта termsAndConditionsAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 978e4ad4941d344d5dcb4da2e5557a4c8eaacb60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971859"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="a0fae-103">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="a0fae-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="a0fae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0fae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0fae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0fae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0fae-106">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0fae-106">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0fae-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a0fae-107">Prerequisites</span></span>
<span data-ttu-id="a0fae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0fae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0fae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0fae-110">Permission type</span></span>|<span data-ttu-id="a0fae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0fae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0fae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0fae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0fae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0fae-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a0fae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0fae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0fae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0fae-115">Not supported.</span></span>|
|<span data-ttu-id="a0fae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0fae-116">Application</span></span>|<span data-ttu-id="a0fae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0fae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0fae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0fae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0fae-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0fae-119">Optional query parameters</span></span>
<span data-ttu-id="a0fae-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0fae-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0fae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0fae-121">Request headers</span></span>
|<span data-ttu-id="a0fae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0fae-122">Header</span></span>|<span data-ttu-id="a0fae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a0fae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0fae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0fae-124">Authorization</span></span>|<span data-ttu-id="a0fae-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0fae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0fae-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a0fae-126">Accept</span></span>|<span data-ttu-id="a0fae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0fae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0fae-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0fae-128">Request body</span></span>
<span data-ttu-id="a0fae-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0fae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0fae-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0fae-130">Response</span></span>
<span data-ttu-id="a0fae-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0fae-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0fae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a0fae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0fae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0fae-133">Request</span></span>
<span data-ttu-id="a0fae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0fae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a0fae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0fae-135">Response</span></span>
<span data-ttu-id="a0fae-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0fae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





