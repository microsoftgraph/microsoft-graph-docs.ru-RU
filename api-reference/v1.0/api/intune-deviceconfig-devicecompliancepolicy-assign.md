---
title: Действие assign
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b25039710d8f9382c5946bcb24c7c0a7a7c80af1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354275"
---
# <a name="assign-action"></a><span data-ttu-id="11519-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="11519-103">assign action</span></span>

> <span data-ttu-id="11519-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11519-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11519-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="11519-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11519-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11519-106">Prerequisites</span></span>
<span data-ttu-id="11519-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11519-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11519-109">Permission type</span></span>|<span data-ttu-id="11519-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11519-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11519-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11519-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11519-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11519-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11519-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11519-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11519-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11519-114">Not supported.</span></span>|
|<span data-ttu-id="11519-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11519-115">Application</span></span>|<span data-ttu-id="11519-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11519-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11519-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11519-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="11519-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11519-118">Request headers</span></span>
|<span data-ttu-id="11519-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11519-119">Header</span></span>|<span data-ttu-id="11519-120">Значение</span><span class="sxs-lookup"><span data-stu-id="11519-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11519-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11519-121">Authorization</span></span>|<span data-ttu-id="11519-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11519-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11519-123">Accept</span><span class="sxs-lookup"><span data-stu-id="11519-123">Accept</span></span>|<span data-ttu-id="11519-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11519-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11519-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11519-125">Request body</span></span>
<span data-ttu-id="11519-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11519-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="11519-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="11519-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="11519-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="11519-128">Property</span></span>|<span data-ttu-id="11519-129">Тип</span><span class="sxs-lookup"><span data-stu-id="11519-129">Type</span></span>|<span data-ttu-id="11519-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11519-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11519-131">assignments</span><span class="sxs-lookup"><span data-stu-id="11519-131">assignments</span></span>|<span data-ttu-id="11519-132">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11519-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="11519-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11519-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="11519-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="11519-134">Response</span></span>
<span data-ttu-id="11519-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11519-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11519-136">Пример</span><span class="sxs-lookup"><span data-stu-id="11519-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="11519-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="11519-137">Request</span></span>
<span data-ttu-id="11519-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11519-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11519-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="11519-139">Response</span></span>
<span data-ttu-id="11519-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11519-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




