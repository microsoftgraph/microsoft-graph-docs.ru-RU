---
title: Получение объекта termsAndConditionsAssignment
description: Чтение свойств и связей объекта termsAndConditionsAssignment.
author: tfitzmac
ms.openlocfilehash: eb0f56703e50a48966dc2a8c27aa6a66e5fbdb6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319441"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="5e726-103">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5e726-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="5e726-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e726-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e726-105">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5e726-105">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e726-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e726-106">Prerequisites</span></span>
<span data-ttu-id="5e726-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e726-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e726-109">Permission type</span></span>|<span data-ttu-id="5e726-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e726-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e726-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e726-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e726-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e726-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5e726-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e726-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e726-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e726-114">Not supported.</span></span>|
|<span data-ttu-id="5e726-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e726-115">Application</span></span>|<span data-ttu-id="5e726-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e726-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e726-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e726-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e726-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e726-118">Optional query parameters</span></span>
<span data-ttu-id="5e726-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e726-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5e726-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e726-120">Request headers</span></span>
|<span data-ttu-id="5e726-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e726-121">Header</span></span>|<span data-ttu-id="5e726-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e726-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e726-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e726-123">Authorization</span></span>|<span data-ttu-id="5e726-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e726-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e726-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e726-125">Accept</span></span>|<span data-ttu-id="5e726-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e726-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e726-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e726-127">Request body</span></span>
<span data-ttu-id="5e726-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e726-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e726-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e726-129">Response</span></span>
<span data-ttu-id="5e726-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e726-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e726-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5e726-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e726-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e726-132">Request</span></span>
<span data-ttu-id="5e726-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e726-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5e726-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e726-134">Response</span></span>
<span data-ttu-id="5e726-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e726-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



