---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f203b0a4d12dfd3124e359210f13527b8e8b8401
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443176"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="3ce0b-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="3ce0b-103">Create deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="3ce0b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3ce0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ce0b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ce0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ce0b-107">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="3ce0b-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ce0b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3ce0b-108">Prerequisites</span></span>
<span data-ttu-id="3ce0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ce0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ce0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ce0b-111">Permission type</span></span>|<span data-ttu-id="3ce0b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ce0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ce0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ce0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ce0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ce0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ce0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ce0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-116">Not supported.</span></span>|
|<span data-ttu-id="3ce0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ce0b-117">Application</span></span>|<span data-ttu-id="3ce0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ce0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ce0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="3ce0b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ce0b-120">Request headers</span></span>
|<span data-ttu-id="3ce0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ce0b-121">Header</span></span>|<span data-ttu-id="3ce0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ce0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ce0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce0b-123">Authorization</span></span>|<span data-ttu-id="3ce0b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ce0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ce0b-125">Accept</span></span>|<span data-ttu-id="3ce0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ce0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ce0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ce0b-127">Request body</span></span>
<span data-ttu-id="3ce0b-128">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="3ce0b-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="3ce0b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ce0b-130">Property</span></span>|<span data-ttu-id="3ce0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3ce0b-131">Type</span></span>|<span data-ttu-id="3ce0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3ce0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ce0b-133">id</span><span class="sxs-lookup"><span data-stu-id="3ce0b-133">id</span></span>|<span data-ttu-id="3ce0b-134">String</span><span class="sxs-lookup"><span data-stu-id="3ce0b-134">String</span></span>|<span data-ttu-id="3ce0b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-135">Key of the entity.</span></span>|
|<span data-ttu-id="3ce0b-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="3ce0b-136">ruleName</span></span>|<span data-ttu-id="3ce0b-137">String</span><span class="sxs-lookup"><span data-stu-id="3ce0b-137">String</span></span>|<span data-ttu-id="3ce0b-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="3ce0b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ce0b-139">Response</span></span>
<span data-ttu-id="3ce0b-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce0b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3ce0b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ce0b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ce0b-142">Request</span></span>
<span data-ttu-id="3ce0b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="3ce0b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ce0b-144">Response</span></span>
<span data-ttu-id="3ce0b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ce0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





