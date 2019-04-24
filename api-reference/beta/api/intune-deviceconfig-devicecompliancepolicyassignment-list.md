---
title: Перечисление объектов deviceCompliancePolicyAssignment
description: Список свойств и связей объектов deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20c80c4213c37075ee280093c0016883f4d9bce7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32470463"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="01359-103">Перечисление объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="01359-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="01359-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01359-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01359-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01359-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01359-106">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="01359-106">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01359-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01359-107">Prerequisites</span></span>
<span data-ttu-id="01359-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01359-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01359-110">Permission type</span></span>|<span data-ttu-id="01359-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01359-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01359-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01359-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01359-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="01359-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="01359-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01359-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01359-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01359-115">Not supported.</span></span>|
|<span data-ttu-id="01359-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01359-116">Application</span></span>|<span data-ttu-id="01359-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01359-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01359-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01359-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="01359-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01359-119">Request headers</span></span>
|<span data-ttu-id="01359-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01359-120">Header</span></span>|<span data-ttu-id="01359-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01359-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01359-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01359-122">Authorization</span></span>|<span data-ttu-id="01359-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01359-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01359-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01359-124">Accept</span></span>|<span data-ttu-id="01359-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01359-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01359-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01359-126">Request body</span></span>
<span data-ttu-id="01359-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01359-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01359-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="01359-128">Response</span></span>
<span data-ttu-id="01359-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01359-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01359-130">Пример</span><span class="sxs-lookup"><span data-stu-id="01359-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="01359-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="01359-131">Request</span></span>
<span data-ttu-id="01359-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01359-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="01359-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="01359-133">Response</span></span>
<span data-ttu-id="01359-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01359-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





