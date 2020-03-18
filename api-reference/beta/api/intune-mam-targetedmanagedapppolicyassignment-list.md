---
title: Перечисление объектов targetedManagedAppPolicyAssignment
description: Список свойств и связей объектов targetedManagedAppPolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb92f68efef8a9caead4365a5bc7fbdb7774a098
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803423"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="c1560-103">Перечисление объектов targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="c1560-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="c1560-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1560-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1560-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1560-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1560-106">Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c1560-106">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1560-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1560-107">Prerequisites</span></span>
<span data-ttu-id="c1560-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1560-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1560-110">Permission type</span></span>|<span data-ttu-id="c1560-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1560-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1560-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1560-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1560-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1560-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1560-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1560-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1560-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1560-115">Not supported.</span></span>|
|<span data-ttu-id="c1560-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1560-116">Application</span></span>|<span data-ttu-id="c1560-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1560-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1560-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1560-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c1560-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1560-119">Request headers</span></span>
|<span data-ttu-id="c1560-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1560-120">Header</span></span>|<span data-ttu-id="c1560-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1560-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1560-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1560-122">Authorization</span></span>|<span data-ttu-id="c1560-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1560-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1560-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c1560-124">Accept</span></span>|<span data-ttu-id="c1560-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1560-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1560-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1560-126">Request body</span></span>
<span data-ttu-id="c1560-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1560-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1560-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1560-128">Response</span></span>
<span data-ttu-id="c1560-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1560-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1560-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c1560-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1560-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1560-131">Request</span></span>
<span data-ttu-id="c1560-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1560-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="c1560-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1560-133">Response</span></span>
<span data-ttu-id="c1560-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1560-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




