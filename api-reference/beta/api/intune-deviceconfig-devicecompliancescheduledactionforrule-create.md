---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fca9632f3ef41756e6e903005770f20bf3a200f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074701"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="14a05-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="14a05-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="14a05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14a05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14a05-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14a05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14a05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14a05-107">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="14a05-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14a05-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14a05-108">Prerequisites</span></span>
<span data-ttu-id="14a05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14a05-111">Permission type</span></span>|<span data-ttu-id="14a05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14a05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14a05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14a05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14a05-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a05-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14a05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14a05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14a05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a05-116">Not supported.</span></span>|
|<span data-ttu-id="14a05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14a05-117">Application</span></span>|<span data-ttu-id="14a05-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a05-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14a05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14a05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="14a05-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14a05-120">Request headers</span></span>
|<span data-ttu-id="14a05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14a05-121">Header</span></span>|<span data-ttu-id="14a05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14a05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14a05-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14a05-123">Authorization</span></span>|<span data-ttu-id="14a05-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14a05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14a05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14a05-125">Accept</span></span>|<span data-ttu-id="14a05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14a05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14a05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14a05-127">Request body</span></span>
<span data-ttu-id="14a05-128">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14a05-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="14a05-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="14a05-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="14a05-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14a05-130">Property</span></span>|<span data-ttu-id="14a05-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14a05-131">Type</span></span>|<span data-ttu-id="14a05-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14a05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14a05-133">id</span><span class="sxs-lookup"><span data-stu-id="14a05-133">id</span></span>|<span data-ttu-id="14a05-134">String</span><span class="sxs-lookup"><span data-stu-id="14a05-134">String</span></span>|<span data-ttu-id="14a05-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14a05-135">Key of the entity.</span></span>|
|<span data-ttu-id="14a05-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="14a05-136">ruleName</span></span>|<span data-ttu-id="14a05-137">String</span><span class="sxs-lookup"><span data-stu-id="14a05-137">String</span></span>|<span data-ttu-id="14a05-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="14a05-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="14a05-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="14a05-139">Response</span></span>
<span data-ttu-id="14a05-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14a05-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a05-141">Пример</span><span class="sxs-lookup"><span data-stu-id="14a05-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="14a05-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="14a05-142">Request</span></span>
<span data-ttu-id="14a05-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14a05-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="14a05-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="14a05-144">Response</span></span>
<span data-ttu-id="14a05-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14a05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






