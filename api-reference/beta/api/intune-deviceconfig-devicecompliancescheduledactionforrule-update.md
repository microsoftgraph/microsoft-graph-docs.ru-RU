---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 072ea9e0c210742aead5e7681796b7791ff5efef
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791392"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="cb8c8-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="cb8c8-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="cb8c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb8c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb8c8-106">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="cb8c8-106">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb8c8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb8c8-107">Prerequisites</span></span>
<span data-ttu-id="cb8c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb8c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb8c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb8c8-110">Permission type</span></span>|<span data-ttu-id="cb8c8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb8c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb8c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb8c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb8c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb8c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb8c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb8c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-115">Not supported.</span></span>|
|<span data-ttu-id="cb8c8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb8c8-116">Application</span></span>|<span data-ttu-id="cb8c8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb8c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb8c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="cb8c8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb8c8-119">Request headers</span></span>
|<span data-ttu-id="cb8c8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb8c8-120">Header</span></span>|<span data-ttu-id="cb8c8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cb8c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb8c8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb8c8-122">Authorization</span></span>|<span data-ttu-id="cb8c8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb8c8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cb8c8-124">Accept</span></span>|<span data-ttu-id="cb8c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb8c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb8c8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb8c8-126">Request body</span></span>
<span data-ttu-id="cb8c8-127">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-127">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="cb8c8-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="cb8c8-128">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="cb8c8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb8c8-129">Property</span></span>|<span data-ttu-id="cb8c8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cb8c8-130">Type</span></span>|<span data-ttu-id="cb8c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cb8c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb8c8-132">id</span><span class="sxs-lookup"><span data-stu-id="cb8c8-132">id</span></span>|<span data-ttu-id="cb8c8-133">String</span><span class="sxs-lookup"><span data-stu-id="cb8c8-133">String</span></span>|<span data-ttu-id="cb8c8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-134">Key of the entity.</span></span>|
|<span data-ttu-id="cb8c8-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="cb8c8-135">ruleName</span></span>|<span data-ttu-id="cb8c8-136">String</span><span class="sxs-lookup"><span data-stu-id="cb8c8-136">String</span></span>|<span data-ttu-id="cb8c8-137">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="cb8c8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb8c8-138">Response</span></span>
<span data-ttu-id="cb8c8-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-139">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb8c8-140">Пример</span><span class="sxs-lookup"><span data-stu-id="cb8c8-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb8c8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb8c8-141">Request</span></span>
<span data-ttu-id="cb8c8-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="cb8c8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb8c8-143">Response</span></span>
<span data-ttu-id="cb8c8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb8c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





