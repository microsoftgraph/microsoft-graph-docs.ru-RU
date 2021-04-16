---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f69f7c73f13b8b515dcfc8538e1d6689c7a542b2
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863396"
---
# <a name="assign-action"></a><span data-ttu-id="0a162-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="0a162-103">assign action</span></span>

<span data-ttu-id="0a162-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a162-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a162-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a162-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a162-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a162-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0a162-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a162-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0a162-108">Prerequisites</span></span>
<span data-ttu-id="0a162-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a162-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a162-111">Permission type</span></span>|<span data-ttu-id="0a162-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a162-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a162-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a162-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0a162-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="0a162-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0a162-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a162-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a162-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a162-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a162-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a162-117">Not supported.</span></span>|
|<span data-ttu-id="0a162-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0a162-118">Application</span></span>||
| <span data-ttu-id="0a162-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="0a162-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0a162-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a162-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a162-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a162-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0a162-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a162-122">Request headers</span></span>
|<span data-ttu-id="0a162-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a162-123">Header</span></span>|<span data-ttu-id="0a162-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0a162-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a162-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a162-125">Authorization</span></span>|<span data-ttu-id="0a162-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a162-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a162-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0a162-127">Accept</span></span>|<span data-ttu-id="0a162-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0a162-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a162-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a162-129">Request body</span></span>
<span data-ttu-id="0a162-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a162-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a162-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0a162-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a162-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a162-132">Property</span></span>|<span data-ttu-id="0a162-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0a162-133">Type</span></span>|<span data-ttu-id="0a162-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0a162-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a162-135">assignments</span><span class="sxs-lookup"><span data-stu-id="0a162-135">assignments</span></span>|<span data-ttu-id="0a162-136">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0a162-136">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="0a162-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0a162-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a162-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a162-138">Response</span></span>
<span data-ttu-id="0a162-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a162-139">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a162-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0a162-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a162-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a162-141">Request</span></span>
<span data-ttu-id="0a162-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a162-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="0a162-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a162-143">Response</span></span>
<span data-ttu-id="0a162-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a162-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







