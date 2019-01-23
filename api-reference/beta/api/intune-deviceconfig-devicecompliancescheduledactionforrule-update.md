---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2ae868b5c11220423c4f1ee496c77f8cd0482c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414643"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="4c9f7-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="4c9f7-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="4c9f7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4c9f7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c9f7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c9f7-107">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="4c9f7-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c9f7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c9f7-108">Prerequisites</span></span>
<span data-ttu-id="4c9f7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c9f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c9f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c9f7-111">Permission type</span></span>|<span data-ttu-id="4c9f7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c9f7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c9f7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c9f7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c9f7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c9f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-116">Not supported.</span></span>|
|<span data-ttu-id="4c9f7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c9f7-117">Application</span></span>|<span data-ttu-id="4c9f7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c9f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c9f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="4c9f7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c9f7-120">Request headers</span></span>
|<span data-ttu-id="4c9f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c9f7-121">Header</span></span>|<span data-ttu-id="4c9f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c9f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c9f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c9f7-123">Authorization</span></span>|<span data-ttu-id="4c9f7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c9f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c9f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c9f7-125">Accept</span></span>|<span data-ttu-id="4c9f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c9f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c9f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c9f7-127">Request body</span></span>
<span data-ttu-id="4c9f7-128">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="4c9f7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="4c9f7-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="4c9f7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c9f7-130">Property</span></span>|<span data-ttu-id="4c9f7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c9f7-131">Type</span></span>|<span data-ttu-id="4c9f7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c9f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c9f7-133">id</span><span class="sxs-lookup"><span data-stu-id="4c9f7-133">id</span></span>|<span data-ttu-id="4c9f7-134">String</span><span class="sxs-lookup"><span data-stu-id="4c9f7-134">String</span></span>|<span data-ttu-id="4c9f7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-135">Key of the entity.</span></span>|
|<span data-ttu-id="4c9f7-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="4c9f7-136">ruleName</span></span>|<span data-ttu-id="4c9f7-137">String</span><span class="sxs-lookup"><span data-stu-id="4c9f7-137">String</span></span>|<span data-ttu-id="4c9f7-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="4c9f7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c9f7-139">Response</span></span>
<span data-ttu-id="4c9f7-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c9f7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4c9f7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c9f7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c9f7-142">Request</span></span>
<span data-ttu-id="4c9f7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="4c9f7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c9f7-144">Response</span></span>
<span data-ttu-id="4c9f7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c9f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




