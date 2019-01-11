---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c4f2e985a236f5afa2f36fb4a9fc41230764d45c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822920"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="74d08-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="74d08-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="74d08-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74d08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74d08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74d08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74d08-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74d08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74d08-107">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="74d08-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74d08-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="74d08-108">Prerequisites</span></span>
<span data-ttu-id="74d08-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74d08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74d08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74d08-111">Permission type</span></span>|<span data-ttu-id="74d08-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74d08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74d08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74d08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74d08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74d08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74d08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74d08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74d08-116">Not supported.</span></span>|
|<span data-ttu-id="74d08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74d08-117">Application</span></span>|<span data-ttu-id="74d08-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74d08-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74d08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74d08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="74d08-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74d08-120">Request headers</span></span>
|<span data-ttu-id="74d08-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74d08-121">Header</span></span>|<span data-ttu-id="74d08-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74d08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74d08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74d08-123">Authorization</span></span>|<span data-ttu-id="74d08-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="74d08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74d08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74d08-125">Accept</span></span>|<span data-ttu-id="74d08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74d08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74d08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74d08-127">Request body</span></span>
<span data-ttu-id="74d08-128">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74d08-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="74d08-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="74d08-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="74d08-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74d08-130">Property</span></span>|<span data-ttu-id="74d08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74d08-131">Type</span></span>|<span data-ttu-id="74d08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74d08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74d08-133">id</span><span class="sxs-lookup"><span data-stu-id="74d08-133">id</span></span>|<span data-ttu-id="74d08-134">Строка</span><span class="sxs-lookup"><span data-stu-id="74d08-134">String</span></span>|<span data-ttu-id="74d08-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="74d08-135">Key of the entity.</span></span>|
|<span data-ttu-id="74d08-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="74d08-136">ruleName</span></span>|<span data-ttu-id="74d08-137">String</span><span class="sxs-lookup"><span data-stu-id="74d08-137">String</span></span>|<span data-ttu-id="74d08-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="74d08-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="74d08-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="74d08-139">Response</span></span>
<span data-ttu-id="74d08-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74d08-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74d08-141">Пример</span><span class="sxs-lookup"><span data-stu-id="74d08-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="74d08-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="74d08-142">Request</span></span>
<span data-ttu-id="74d08-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74d08-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 37

{
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="74d08-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="74d08-144">Response</span></span>
<span data-ttu-id="74d08-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74d08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





