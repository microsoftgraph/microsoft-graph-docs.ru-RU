---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 145ecb6fcad6313dd221df16cc63f501e762669f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083374"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="68f42-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="68f42-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="68f42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68f42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68f42-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68f42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68f42-106">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="68f42-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68f42-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="68f42-107">Prerequisites</span></span>
<span data-ttu-id="68f42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68f42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68f42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68f42-110">Permission type</span></span>|<span data-ttu-id="68f42-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68f42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68f42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68f42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68f42-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68f42-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68f42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68f42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68f42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68f42-115">Not supported.</span></span>|
|<span data-ttu-id="68f42-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68f42-116">Application</span></span>|<span data-ttu-id="68f42-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68f42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68f42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68f42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="68f42-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68f42-119">Request headers</span></span>
|<span data-ttu-id="68f42-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68f42-120">Header</span></span>|<span data-ttu-id="68f42-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68f42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68f42-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68f42-122">Authorization</span></span>|<span data-ttu-id="68f42-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68f42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68f42-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68f42-124">Accept</span></span>|<span data-ttu-id="68f42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68f42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68f42-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68f42-126">Request body</span></span>
<span data-ttu-id="68f42-127">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68f42-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="68f42-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="68f42-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="68f42-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="68f42-129">Property</span></span>|<span data-ttu-id="68f42-130">Тип</span><span class="sxs-lookup"><span data-stu-id="68f42-130">Type</span></span>|<span data-ttu-id="68f42-131">Описание</span><span class="sxs-lookup"><span data-stu-id="68f42-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f42-132">id</span><span class="sxs-lookup"><span data-stu-id="68f42-132">id</span></span>|<span data-ttu-id="68f42-133">Строка</span><span class="sxs-lookup"><span data-stu-id="68f42-133">String</span></span>|<span data-ttu-id="68f42-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68f42-134">Key of the entity.</span></span>|
|<span data-ttu-id="68f42-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="68f42-135">ruleName</span></span>|<span data-ttu-id="68f42-136">String</span><span class="sxs-lookup"><span data-stu-id="68f42-136">String</span></span>|<span data-ttu-id="68f42-137">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="68f42-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="68f42-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f42-138">Response</span></span>
<span data-ttu-id="68f42-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68f42-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68f42-140">Пример</span><span class="sxs-lookup"><span data-stu-id="68f42-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="68f42-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="68f42-141">Request</span></span>
<span data-ttu-id="68f42-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68f42-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="68f42-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f42-143">Response</span></span>
<span data-ttu-id="68f42-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68f42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









