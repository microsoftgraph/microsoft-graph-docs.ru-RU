---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c20abd628b3f919924fe2d75a8df485157ab2ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083507"
---
# <a name="assign-action"></a><span data-ttu-id="40192-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="40192-103">assign action</span></span>

<span data-ttu-id="40192-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40192-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40192-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40192-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="40192-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40192-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40192-107">Prerequisites</span></span>
<span data-ttu-id="40192-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40192-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40192-110">Permission type</span></span>|<span data-ttu-id="40192-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40192-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40192-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40192-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40192-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40192-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40192-115">Not supported.</span></span>|
|<span data-ttu-id="40192-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40192-116">Application</span></span>|<span data-ttu-id="40192-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40192-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40192-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="40192-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40192-119">Request headers</span></span>
|<span data-ttu-id="40192-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40192-120">Header</span></span>|<span data-ttu-id="40192-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40192-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40192-122">Authorization</span></span>|<span data-ttu-id="40192-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40192-124">Accept</span><span class="sxs-lookup"><span data-stu-id="40192-124">Accept</span></span>|<span data-ttu-id="40192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40192-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40192-126">Request body</span></span>
<span data-ttu-id="40192-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40192-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="40192-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="40192-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="40192-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="40192-129">Property</span></span>|<span data-ttu-id="40192-130">Тип</span><span class="sxs-lookup"><span data-stu-id="40192-130">Type</span></span>|<span data-ttu-id="40192-131">Описание</span><span class="sxs-lookup"><span data-stu-id="40192-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40192-132">assignments</span><span class="sxs-lookup"><span data-stu-id="40192-132">assignments</span></span>|<span data-ttu-id="40192-133">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="40192-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="40192-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="40192-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40192-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40192-135">Response</span></span>
<span data-ttu-id="40192-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40192-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40192-137">Пример</span><span class="sxs-lookup"><span data-stu-id="40192-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="40192-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="40192-138">Request</span></span>
<span data-ttu-id="40192-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40192-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="40192-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="40192-140">Response</span></span>
<span data-ttu-id="40192-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40192-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









