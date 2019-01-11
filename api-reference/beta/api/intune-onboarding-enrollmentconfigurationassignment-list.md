---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8691d2b05e7fe618c5ed7d3d4fd6ea314467e7fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849653"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="b6324-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b6324-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="b6324-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6324-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6324-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6324-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6324-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6324-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6324-107">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6324-107">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6324-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b6324-108">Prerequisites</span></span>
<span data-ttu-id="b6324-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6324-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6324-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6324-111">Permission type</span></span>|<span data-ttu-id="b6324-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6324-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6324-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6324-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6324-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b6324-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6324-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6324-116">Not supported.</span></span>|
|<span data-ttu-id="b6324-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6324-117">Application</span></span>|<span data-ttu-id="b6324-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6324-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6324-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b6324-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6324-120">Request headers</span></span>
|<span data-ttu-id="b6324-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6324-121">Header</span></span>|<span data-ttu-id="b6324-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6324-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6324-123">Authorization</span></span>|<span data-ttu-id="b6324-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6324-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6324-125">Accept</span></span>|<span data-ttu-id="b6324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6324-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6324-127">Request body</span></span>
<span data-ttu-id="b6324-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6324-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6324-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6324-129">Response</span></span>
<span data-ttu-id="b6324-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6324-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6324-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b6324-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6324-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6324-132">Request</span></span>
<span data-ttu-id="b6324-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6324-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="b6324-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6324-134">Response</span></span>
<span data-ttu-id="b6324-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b6324-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





