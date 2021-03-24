---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acf3e522b29fe1783b7480368a82323f13c566c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128203"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="2c057-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="2c057-103">Update deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="2c057-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c057-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c057-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c057-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c057-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c057-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c057-107">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="2c057-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c057-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2c057-108">Prerequisites</span></span>
<span data-ttu-id="2c057-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c057-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c057-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c057-111">Permission type</span></span>|<span data-ttu-id="2c057-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c057-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c057-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c057-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c057-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c057-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c057-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c057-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c057-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c057-116">Not supported.</span></span>|
|<span data-ttu-id="2c057-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2c057-117">Application</span></span>|<span data-ttu-id="2c057-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c057-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c057-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c057-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="2c057-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2c057-120">Request headers</span></span>
|<span data-ttu-id="2c057-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c057-121">Header</span></span>|<span data-ttu-id="2c057-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2c057-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c057-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c057-123">Authorization</span></span>|<span data-ttu-id="2c057-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c057-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c057-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c057-125">Accept</span></span>|<span data-ttu-id="2c057-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c057-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c057-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c057-127">Request body</span></span>
<span data-ttu-id="2c057-128">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c057-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="2c057-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="2c057-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="2c057-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c057-130">Property</span></span>|<span data-ttu-id="2c057-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2c057-131">Type</span></span>|<span data-ttu-id="2c057-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c057-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c057-133">id</span><span class="sxs-lookup"><span data-stu-id="2c057-133">id</span></span>|<span data-ttu-id="2c057-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2c057-134">String</span></span>|<span data-ttu-id="2c057-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2c057-135">Key of the entity.</span></span>|
|<span data-ttu-id="2c057-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="2c057-136">ruleName</span></span>|<span data-ttu-id="2c057-137">String</span><span class="sxs-lookup"><span data-stu-id="2c057-137">String</span></span>|<span data-ttu-id="2c057-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="2c057-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="2c057-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c057-139">Response</span></span>
<span data-ttu-id="2c057-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c057-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c057-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2c057-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c057-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c057-142">Request</span></span>
<span data-ttu-id="2c057-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c057-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="2c057-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c057-144">Response</span></span>
<span data-ttu-id="2c057-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c057-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




