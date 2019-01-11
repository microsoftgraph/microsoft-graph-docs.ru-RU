---
title: Перечисление объектов targetedManagedAppPolicyAssignment
description: Список свойств и связей объектов targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a9ed6fd48467408ba940157530d8b9925515f3d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822003"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="ffbe1-103">Перечисление объектов targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ffbe1-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="ffbe1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffbe1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffbe1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffbe1-107">Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffbe1-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffbe1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ffbe1-108">Prerequisites</span></span>
<span data-ttu-id="ffbe1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffbe1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffbe1-111">Permission type</span></span>|<span data-ttu-id="ffbe1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffbe1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffbe1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffbe1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffbe1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffbe1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ffbe1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffbe1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffbe1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-116">Not supported.</span></span>|
|<span data-ttu-id="ffbe1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffbe1-117">Application</span></span>|<span data-ttu-id="ffbe1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffbe1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffbe1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ffbe1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffbe1-120">Request headers</span></span>
|<span data-ttu-id="ffbe1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffbe1-121">Header</span></span>|<span data-ttu-id="ffbe1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffbe1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffbe1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffbe1-123">Authorization</span></span>|<span data-ttu-id="ffbe1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ffbe1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffbe1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffbe1-125">Accept</span></span>|<span data-ttu-id="ffbe1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffbe1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffbe1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffbe1-127">Request body</span></span>
<span data-ttu-id="ffbe1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffbe1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffbe1-129">Response</span></span>
<span data-ttu-id="ffbe1-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffbe1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ffbe1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffbe1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffbe1-132">Request</span></span>
<span data-ttu-id="ffbe1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="ffbe1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffbe1-134">Response</span></span>
<span data-ttu-id="ffbe1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





