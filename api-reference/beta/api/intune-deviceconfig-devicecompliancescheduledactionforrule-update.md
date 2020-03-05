---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59aea7c488e93c38beb90ad5a6d6b711cb2fca63
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449259"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="62cf4-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="62cf4-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="62cf4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="62cf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62cf4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62cf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62cf4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62cf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62cf4-107">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="62cf4-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62cf4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="62cf4-108">Prerequisites</span></span>
<span data-ttu-id="62cf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62cf4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62cf4-111">Permission type</span></span>|<span data-ttu-id="62cf4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62cf4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62cf4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62cf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62cf4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cf4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62cf4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62cf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62cf4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62cf4-116">Not supported.</span></span>|
|<span data-ttu-id="62cf4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62cf4-117">Application</span></span>|<span data-ttu-id="62cf4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cf4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62cf4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62cf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="62cf4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="62cf4-120">Request headers</span></span>
|<span data-ttu-id="62cf4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62cf4-121">Header</span></span>|<span data-ttu-id="62cf4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62cf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62cf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62cf4-123">Authorization</span></span>|<span data-ttu-id="62cf4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62cf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62cf4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62cf4-125">Accept</span></span>|<span data-ttu-id="62cf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62cf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62cf4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62cf4-127">Request body</span></span>
<span data-ttu-id="62cf4-128">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62cf4-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="62cf4-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="62cf4-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="62cf4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62cf4-130">Property</span></span>|<span data-ttu-id="62cf4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62cf4-131">Type</span></span>|<span data-ttu-id="62cf4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62cf4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62cf4-133">id</span><span class="sxs-lookup"><span data-stu-id="62cf4-133">id</span></span>|<span data-ttu-id="62cf4-134">String</span><span class="sxs-lookup"><span data-stu-id="62cf4-134">String</span></span>|<span data-ttu-id="62cf4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62cf4-135">Key of the entity.</span></span>|
|<span data-ttu-id="62cf4-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="62cf4-136">ruleName</span></span>|<span data-ttu-id="62cf4-137">String</span><span class="sxs-lookup"><span data-stu-id="62cf4-137">String</span></span>|<span data-ttu-id="62cf4-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="62cf4-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="62cf4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="62cf4-139">Response</span></span>
<span data-ttu-id="62cf4-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62cf4-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62cf4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="62cf4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="62cf4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="62cf4-142">Request</span></span>
<span data-ttu-id="62cf4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62cf4-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="62cf4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="62cf4-144">Response</span></span>
<span data-ttu-id="62cf4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62cf4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





