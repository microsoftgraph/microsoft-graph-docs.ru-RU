---
title: Get targetedManagedAppPolicyAssignment
description: Чтение свойств и связей объекта targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3abec81ea2d39e088c96d2f5d2650010818e4a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807359"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="754f1-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="754f1-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="754f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="754f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="754f1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="754f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="754f1-106">Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="754f1-106">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="754f1-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="754f1-107">Prerequisites</span></span>
<span data-ttu-id="754f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="754f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="754f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="754f1-110">Permission type</span></span>|<span data-ttu-id="754f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="754f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="754f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="754f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="754f1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="754f1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="754f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="754f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="754f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="754f1-115">Not supported.</span></span>|
|<span data-ttu-id="754f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="754f1-116">Application</span></span>|<span data-ttu-id="754f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="754f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="754f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="754f1-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="754f1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="754f1-119">Optional query parameters</span></span>
<span data-ttu-id="754f1-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="754f1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="754f1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="754f1-121">Request headers</span></span>
|<span data-ttu-id="754f1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="754f1-122">Header</span></span>|<span data-ttu-id="754f1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="754f1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="754f1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="754f1-124">Authorization</span></span>|<span data-ttu-id="754f1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="754f1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="754f1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="754f1-126">Accept</span></span>|<span data-ttu-id="754f1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="754f1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="754f1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="754f1-128">Request body</span></span>
<span data-ttu-id="754f1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="754f1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="754f1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="754f1-130">Response</span></span>
<span data-ttu-id="754f1-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="754f1-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="754f1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="754f1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="754f1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="754f1-133">Request</span></span>
<span data-ttu-id="754f1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="754f1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="754f1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="754f1-135">Response</span></span>
<span data-ttu-id="754f1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="754f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





