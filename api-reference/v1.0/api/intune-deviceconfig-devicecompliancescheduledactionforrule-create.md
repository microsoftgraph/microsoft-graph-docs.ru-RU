---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14ecd6ad49c2a51287fcf0b6de8cc75853ab4847
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399733"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="61e17-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="61e17-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="61e17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61e17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61e17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61e17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61e17-106">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="61e17-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61e17-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="61e17-107">Prerequisites</span></span>
<span data-ttu-id="61e17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61e17-110">Permission type</span></span>|<span data-ttu-id="61e17-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61e17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61e17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61e17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61e17-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e17-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61e17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61e17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61e17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61e17-115">Not supported.</span></span>|
|<span data-ttu-id="61e17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61e17-116">Application</span></span>|<span data-ttu-id="61e17-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61e17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61e17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61e17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="61e17-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="61e17-119">Request headers</span></span>
|<span data-ttu-id="61e17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61e17-120">Header</span></span>|<span data-ttu-id="61e17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="61e17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61e17-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61e17-122">Authorization</span></span>|<span data-ttu-id="61e17-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61e17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61e17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="61e17-124">Accept</span></span>|<span data-ttu-id="61e17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61e17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61e17-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61e17-126">Request body</span></span>
<span data-ttu-id="61e17-127">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61e17-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="61e17-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="61e17-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="61e17-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="61e17-129">Property</span></span>|<span data-ttu-id="61e17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="61e17-130">Type</span></span>|<span data-ttu-id="61e17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="61e17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61e17-132">id</span><span class="sxs-lookup"><span data-stu-id="61e17-132">id</span></span>|<span data-ttu-id="61e17-133">String</span><span class="sxs-lookup"><span data-stu-id="61e17-133">String</span></span>|<span data-ttu-id="61e17-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="61e17-134">Key of the entity.</span></span>|
|<span data-ttu-id="61e17-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="61e17-135">ruleName</span></span>|<span data-ttu-id="61e17-136">String</span><span class="sxs-lookup"><span data-stu-id="61e17-136">String</span></span>|<span data-ttu-id="61e17-137">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="61e17-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="61e17-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e17-138">Response</span></span>
<span data-ttu-id="61e17-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61e17-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61e17-140">Пример</span><span class="sxs-lookup"><span data-stu-id="61e17-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="61e17-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="61e17-141">Request</span></span>
<span data-ttu-id="61e17-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61e17-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="61e17-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e17-143">Response</span></span>
<span data-ttu-id="61e17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61e17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```






