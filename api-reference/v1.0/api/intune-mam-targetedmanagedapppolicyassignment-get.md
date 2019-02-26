---
title: Get targetedManagedAppPolicyAssignment
description: Чтение свойств и связей объекта targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8956cb9b3877fa3f53ce65b306b8d1384ad12b8d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259999"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="ae4bc-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ae4bc-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="ae4bc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae4bc-105">Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ae4bc-105">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae4bc-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ae4bc-106">Prerequisites</span></span>
<span data-ttu-id="ae4bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae4bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae4bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae4bc-109">Permission type</span></span>|<span data-ttu-id="ae4bc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae4bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae4bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae4bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ae4bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae4bc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ae4bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae4bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae4bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-114">Not supported.</span></span>|
|<span data-ttu-id="ae4bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae4bc-115">Application</span></span>|<span data-ttu-id="ae4bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae4bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae4bc-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="ae4bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae4bc-118">Optional query parameters</span></span>
<span data-ttu-id="ae4bc-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae4bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae4bc-120">Request headers</span></span>
|<span data-ttu-id="ae4bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae4bc-121">Header</span></span>|<span data-ttu-id="ae4bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae4bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae4bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae4bc-123">Authorization</span></span>|<span data-ttu-id="ae4bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ae4bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae4bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae4bc-125">Accept</span></span>|<span data-ttu-id="ae4bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae4bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae4bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae4bc-127">Request body</span></span>
<span data-ttu-id="ae4bc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae4bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae4bc-129">Response</span></span>
<span data-ttu-id="ae4bc-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae4bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ae4bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae4bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae4bc-132">Request</span></span>
<span data-ttu-id="ae4bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ae4bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae4bc-134">Response</span></span>
<span data-ttu-id="ae4bc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae4bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



