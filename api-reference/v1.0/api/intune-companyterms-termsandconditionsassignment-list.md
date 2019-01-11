---
title: Перечисление объектов termsAndConditionsAssignment
description: Список свойств и связей объектов termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0ae712e3fc2d4f4490652c3b74aa69e61df12f0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825055"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="41132-103">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="41132-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="41132-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="41132-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41132-105">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="41132-105">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41132-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41132-106">Prerequisites</span></span>
<span data-ttu-id="41132-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41132-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41132-109">Permission type</span></span>|<span data-ttu-id="41132-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41132-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41132-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41132-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41132-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="41132-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="41132-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41132-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41132-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41132-114">Not supported.</span></span>|
|<span data-ttu-id="41132-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41132-115">Application</span></span>|<span data-ttu-id="41132-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41132-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41132-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41132-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="41132-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41132-118">Request headers</span></span>
|<span data-ttu-id="41132-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41132-119">Header</span></span>|<span data-ttu-id="41132-120">Значение</span><span class="sxs-lookup"><span data-stu-id="41132-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41132-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41132-121">Authorization</span></span>|<span data-ttu-id="41132-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="41132-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41132-123">Accept</span><span class="sxs-lookup"><span data-stu-id="41132-123">Accept</span></span>|<span data-ttu-id="41132-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41132-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41132-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41132-125">Request body</span></span>
<span data-ttu-id="41132-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41132-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41132-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="41132-127">Response</span></span>
<span data-ttu-id="41132-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41132-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41132-129">Пример</span><span class="sxs-lookup"><span data-stu-id="41132-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="41132-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="41132-130">Request</span></span>
<span data-ttu-id="41132-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41132-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="41132-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="41132-132">Response</span></span>
<span data-ttu-id="41132-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41132-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



