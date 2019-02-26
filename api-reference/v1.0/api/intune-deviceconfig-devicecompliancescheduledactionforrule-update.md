---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adfd70118ba57210b5ac743e6b664b2fe276f98d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257017"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="0eae8-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="0eae8-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="0eae8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eae8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eae8-105">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="0eae8-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eae8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0eae8-106">Prerequisites</span></span>
<span data-ttu-id="0eae8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0eae8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0eae8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eae8-109">Permission type</span></span>|<span data-ttu-id="0eae8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eae8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eae8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eae8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0eae8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eae8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0eae8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eae8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eae8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eae8-114">Not supported.</span></span>|
|<span data-ttu-id="0eae8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eae8-115">Application</span></span>|<span data-ttu-id="0eae8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eae8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eae8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eae8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="0eae8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eae8-118">Request headers</span></span>
|<span data-ttu-id="0eae8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0eae8-119">Header</span></span>|<span data-ttu-id="0eae8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0eae8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eae8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eae8-121">Authorization</span></span>|<span data-ttu-id="0eae8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0eae8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eae8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0eae8-123">Accept</span></span>|<span data-ttu-id="0eae8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0eae8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eae8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eae8-125">Request body</span></span>
<span data-ttu-id="0eae8-126">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eae8-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="0eae8-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="0eae8-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="0eae8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eae8-128">Property</span></span>|<span data-ttu-id="0eae8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0eae8-129">Type</span></span>|<span data-ttu-id="0eae8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0eae8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eae8-131">id</span><span class="sxs-lookup"><span data-stu-id="0eae8-131">id</span></span>|<span data-ttu-id="0eae8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0eae8-132">String</span></span>|<span data-ttu-id="0eae8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0eae8-133">Key of the entity.</span></span>|
|<span data-ttu-id="0eae8-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="0eae8-134">ruleName</span></span>|<span data-ttu-id="0eae8-135">String</span><span class="sxs-lookup"><span data-stu-id="0eae8-135">String</span></span>|<span data-ttu-id="0eae8-136">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="0eae8-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="0eae8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eae8-137">Response</span></span>
<span data-ttu-id="0eae8-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0eae8-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eae8-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0eae8-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eae8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eae8-140">Request</span></span>
<span data-ttu-id="0eae8-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eae8-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="0eae8-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="0eae8-142">Response</span></span>
<span data-ttu-id="0eae8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0eae8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



