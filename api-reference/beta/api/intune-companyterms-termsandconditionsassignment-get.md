---
title: Получение объекта termsAndConditionsAssignment
description: Чтение свойств и связей объекта termsAndConditionsAssignment.
ms.openlocfilehash: 6796ad975e02cfbb290dd234e494307ace7b6f65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075258"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="7f9cb-103">Получение объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f9cb-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="7f9cb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f9cb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f9cb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f9cb-107">Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f9cb-107">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f9cb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f9cb-108">Prerequisites</span></span>
<span data-ttu-id="7f9cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f9cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f9cb-111">Permission type</span></span>|<span data-ttu-id="7f9cb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f9cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f9cb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f9cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f9cb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9cb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7f9cb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f9cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f9cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-116">Not supported.</span></span>|
|<span data-ttu-id="7f9cb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f9cb-117">Application</span></span>|<span data-ttu-id="7f9cb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f9cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f9cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f9cb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f9cb-120">Optional query parameters</span></span>
<span data-ttu-id="7f9cb-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f9cb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f9cb-122">Request headers</span></span>
|<span data-ttu-id="7f9cb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f9cb-123">Header</span></span>|<span data-ttu-id="7f9cb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7f9cb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f9cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f9cb-125">Authorization</span></span>|<span data-ttu-id="7f9cb-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f9cb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f9cb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7f9cb-127">Accept</span></span>|<span data-ttu-id="7f9cb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f9cb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f9cb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f9cb-129">Request body</span></span>
<span data-ttu-id="7f9cb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f9cb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9cb-131">Response</span></span>
<span data-ttu-id="7f9cb-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f9cb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7f9cb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f9cb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f9cb-134">Request</span></span>
<span data-ttu-id="7f9cb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f9cb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7f9cb-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f9cb-136">Response</span></span>
<span data-ttu-id="7f9cb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7f9cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





