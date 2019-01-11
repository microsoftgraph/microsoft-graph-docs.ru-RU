---
title: Get targetedManagedAppPolicyAssignment
description: Чтение свойств и связей объекта targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72515dc491bd6073e94089c1a1747bcebcd986e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846714"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="9b746-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="9b746-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="9b746-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b746-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b746-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b746-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b746-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9b746-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b746-107">Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9b746-107">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b746-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9b746-108">Prerequisites</span></span>
<span data-ttu-id="9b746-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b746-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b746-111">Permission type</span></span>|<span data-ttu-id="9b746-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b746-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b746-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b746-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b746-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b746-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9b746-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b746-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b746-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b746-116">Not supported.</span></span>|
|<span data-ttu-id="9b746-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b746-117">Application</span></span>|<span data-ttu-id="9b746-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b746-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b746-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b746-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b746-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9b746-120">Optional query parameters</span></span>
<span data-ttu-id="9b746-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9b746-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9b746-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b746-122">Request headers</span></span>
|<span data-ttu-id="9b746-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b746-123">Header</span></span>|<span data-ttu-id="9b746-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9b746-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b746-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b746-125">Authorization</span></span>|<span data-ttu-id="9b746-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9b746-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b746-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9b746-127">Accept</span></span>|<span data-ttu-id="9b746-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9b746-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b746-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b746-129">Request body</span></span>
<span data-ttu-id="9b746-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b746-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b746-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b746-131">Response</span></span>
<span data-ttu-id="9b746-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9b746-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b746-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9b746-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b746-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b746-134">Request</span></span>
<span data-ttu-id="9b746-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b746-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="9b746-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b746-136">Response</span></span>
<span data-ttu-id="9b746-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9b746-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





