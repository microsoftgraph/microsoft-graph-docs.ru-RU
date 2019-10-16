---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2ce1e262bf133bda64d084d9108cc9ec2ef5e39
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536198"
---
# <a name="assign-action"></a><span data-ttu-id="05747-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="05747-103">assign action</span></span>

> <span data-ttu-id="05747-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05747-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05747-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05747-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05747-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05747-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05747-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05747-107">Prerequisites</span></span>
<span data-ttu-id="05747-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05747-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05747-110">Permission type</span></span>|<span data-ttu-id="05747-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05747-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05747-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05747-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="05747-113">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="05747-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="05747-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05747-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05747-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05747-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05747-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05747-116">Not supported.</span></span>|
|<span data-ttu-id="05747-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="05747-117">Application</span></span>||
| <span data-ttu-id="05747-118">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="05747-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="05747-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05747-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05747-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05747-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="05747-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05747-121">Request headers</span></span>
|<span data-ttu-id="05747-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05747-122">Header</span></span>|<span data-ttu-id="05747-123">Значение</span><span class="sxs-lookup"><span data-stu-id="05747-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05747-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05747-124">Authorization</span></span>|<span data-ttu-id="05747-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05747-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05747-126">Accept</span><span class="sxs-lookup"><span data-stu-id="05747-126">Accept</span></span>|<span data-ttu-id="05747-127">application/json</span><span class="sxs-lookup"><span data-stu-id="05747-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05747-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05747-128">Request body</span></span>
<span data-ttu-id="05747-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05747-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05747-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="05747-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05747-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="05747-131">Property</span></span>|<span data-ttu-id="05747-132">Тип</span><span class="sxs-lookup"><span data-stu-id="05747-132">Type</span></span>|<span data-ttu-id="05747-133">Описание</span><span class="sxs-lookup"><span data-stu-id="05747-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05747-134">assignments</span><span class="sxs-lookup"><span data-stu-id="05747-134">assignments</span></span>|<span data-ttu-id="05747-135">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="05747-135">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="05747-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05747-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05747-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="05747-137">Response</span></span>
<span data-ttu-id="05747-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05747-138">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05747-139">Пример</span><span class="sxs-lookup"><span data-stu-id="05747-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="05747-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="05747-140">Request</span></span>
<span data-ttu-id="05747-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05747-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05747-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="05747-142">Response</span></span>
<span data-ttu-id="05747-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05747-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






