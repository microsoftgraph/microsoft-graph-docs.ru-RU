---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 564cff7fdbf58eb3e2de09f3d8b6c639c0bff769
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011755"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="ed2ea-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="ed2ea-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="ed2ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed2ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed2ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed2ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed2ea-107">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="ed2ea-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed2ea-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ed2ea-108">Prerequisites</span></span>
<span data-ttu-id="ed2ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed2ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed2ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed2ea-111">Permission type</span></span>|<span data-ttu-id="ed2ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed2ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed2ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed2ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed2ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed2ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed2ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed2ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed2ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-116">Not supported.</span></span>|
|<span data-ttu-id="ed2ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed2ea-117">Application</span></span>|<span data-ttu-id="ed2ea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed2ea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed2ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed2ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="ed2ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ed2ea-120">Request headers</span></span>
|<span data-ttu-id="ed2ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed2ea-121">Header</span></span>|<span data-ttu-id="ed2ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ed2ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed2ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed2ea-123">Authorization</span></span>|<span data-ttu-id="ed2ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed2ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed2ea-125">Accept</span></span>|<span data-ttu-id="ed2ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed2ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed2ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed2ea-127">Request body</span></span>
<span data-ttu-id="ed2ea-128">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="ed2ea-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="ed2ea-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="ed2ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed2ea-130">Property</span></span>|<span data-ttu-id="ed2ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ed2ea-131">Type</span></span>|<span data-ttu-id="ed2ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ed2ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed2ea-133">id</span><span class="sxs-lookup"><span data-stu-id="ed2ea-133">id</span></span>|<span data-ttu-id="ed2ea-134">String</span><span class="sxs-lookup"><span data-stu-id="ed2ea-134">String</span></span>|<span data-ttu-id="ed2ea-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-135">Key of the entity.</span></span>|
|<span data-ttu-id="ed2ea-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="ed2ea-136">ruleName</span></span>|<span data-ttu-id="ed2ea-137">String</span><span class="sxs-lookup"><span data-stu-id="ed2ea-137">String</span></span>|<span data-ttu-id="ed2ea-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="ed2ea-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed2ea-139">Response</span></span>
<span data-ttu-id="ed2ea-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed2ea-141">Пример</span><span class="sxs-lookup"><span data-stu-id="ed2ea-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed2ea-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed2ea-142">Request</span></span>
<span data-ttu-id="ed2ea-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="ed2ea-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed2ea-144">Response</span></span>
<span data-ttu-id="ed2ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed2ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```






