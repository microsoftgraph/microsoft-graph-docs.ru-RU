---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aca544cadaafa2bcc832c2313e98f382528a68b8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755380"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="93a1f-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="93a1f-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="93a1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93a1f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93a1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93a1f-106">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="93a1f-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93a1f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="93a1f-107">Prerequisites</span></span>
<span data-ttu-id="93a1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93a1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93a1f-110">Permission type</span></span>|<span data-ttu-id="93a1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93a1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93a1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93a1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93a1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93a1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93a1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93a1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93a1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a1f-115">Not supported.</span></span>|
|<span data-ttu-id="93a1f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="93a1f-116">Application</span></span>|<span data-ttu-id="93a1f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93a1f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93a1f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93a1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="93a1f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93a1f-119">Request headers</span></span>
|<span data-ttu-id="93a1f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93a1f-120">Header</span></span>|<span data-ttu-id="93a1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="93a1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93a1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93a1f-122">Authorization</span></span>|<span data-ttu-id="93a1f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93a1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93a1f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="93a1f-124">Accept</span></span>|<span data-ttu-id="93a1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93a1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93a1f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93a1f-126">Request body</span></span>
<span data-ttu-id="93a1f-127">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93a1f-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="93a1f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="93a1f-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="93a1f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="93a1f-129">Property</span></span>|<span data-ttu-id="93a1f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="93a1f-130">Type</span></span>|<span data-ttu-id="93a1f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="93a1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93a1f-132">id</span><span class="sxs-lookup"><span data-stu-id="93a1f-132">id</span></span>|<span data-ttu-id="93a1f-133">String</span><span class="sxs-lookup"><span data-stu-id="93a1f-133">String</span></span>|<span data-ttu-id="93a1f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="93a1f-134">Key of the entity.</span></span>|
|<span data-ttu-id="93a1f-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="93a1f-135">ruleName</span></span>|<span data-ttu-id="93a1f-136">String</span><span class="sxs-lookup"><span data-stu-id="93a1f-136">String</span></span>|<span data-ttu-id="93a1f-137">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="93a1f-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="93a1f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="93a1f-138">Response</span></span>
<span data-ttu-id="93a1f-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93a1f-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93a1f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="93a1f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="93a1f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="93a1f-141">Request</span></span>
<span data-ttu-id="93a1f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93a1f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="93a1f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="93a1f-143">Response</span></span>
<span data-ttu-id="93a1f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93a1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




