---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be4fd659bc6dea5c369e8181c071305f3c244f96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459880"
---
# <a name="assign-action"></a><span data-ttu-id="2864f-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="2864f-103">assign action</span></span>

> <span data-ttu-id="2864f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2864f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2864f-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2864f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2864f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2864f-106">Prerequisites</span></span>
<span data-ttu-id="2864f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2864f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2864f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2864f-109">Permission type</span></span>|<span data-ttu-id="2864f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2864f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2864f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2864f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2864f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2864f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2864f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2864f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2864f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2864f-114">Not supported.</span></span>|
|<span data-ttu-id="2864f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2864f-115">Application</span></span>|<span data-ttu-id="2864f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2864f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2864f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2864f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2864f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2864f-118">Request headers</span></span>
|<span data-ttu-id="2864f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2864f-119">Header</span></span>|<span data-ttu-id="2864f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2864f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2864f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2864f-121">Authorization</span></span>|<span data-ttu-id="2864f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2864f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2864f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2864f-123">Accept</span></span>|<span data-ttu-id="2864f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2864f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2864f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2864f-125">Request body</span></span>
<span data-ttu-id="2864f-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2864f-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2864f-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2864f-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2864f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2864f-128">Property</span></span>|<span data-ttu-id="2864f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2864f-129">Type</span></span>|<span data-ttu-id="2864f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2864f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2864f-131">assignments</span><span class="sxs-lookup"><span data-stu-id="2864f-131">assignments</span></span>|<span data-ttu-id="2864f-132">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="2864f-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2864f-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2864f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2864f-134">Response</span></span>
<span data-ttu-id="2864f-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2864f-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2864f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2864f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2864f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2864f-137">Request</span></span>
<span data-ttu-id="2864f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2864f-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2864f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2864f-139">Response</span></span>
<span data-ttu-id="2864f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2864f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



