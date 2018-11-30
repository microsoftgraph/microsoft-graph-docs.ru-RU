---
title: Обновление объекта deviceComplianceScheduledActionForRule
description: Обновление свойств объекта deviceComplianceScheduledActionForRule.
ms.openlocfilehash: d4b6df2d36bfe1852c32e146bb1a553166620a39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025883"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="49eef-103">Обновление объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="49eef-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="49eef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49eef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49eef-105">Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="49eef-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49eef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="49eef-106">Prerequisites</span></span>
<span data-ttu-id="49eef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49eef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49eef-109">Permission type</span></span>|<span data-ttu-id="49eef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49eef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49eef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49eef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49eef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49eef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49eef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49eef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49eef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49eef-114">Not supported.</span></span>|
|<span data-ttu-id="49eef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49eef-115">Application</span></span>|<span data-ttu-id="49eef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49eef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49eef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49eef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="49eef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49eef-118">Request headers</span></span>
|<span data-ttu-id="49eef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49eef-119">Header</span></span>|<span data-ttu-id="49eef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="49eef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49eef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49eef-121">Authorization</span></span>|<span data-ttu-id="49eef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="49eef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49eef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="49eef-123">Accept</span></span>|<span data-ttu-id="49eef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="49eef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49eef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49eef-125">Request body</span></span>
<span data-ttu-id="49eef-126">В тексте запроса добавьте представление объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49eef-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="49eef-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="49eef-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="49eef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="49eef-128">Property</span></span>|<span data-ttu-id="49eef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="49eef-129">Type</span></span>|<span data-ttu-id="49eef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="49eef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49eef-131">id</span><span class="sxs-lookup"><span data-stu-id="49eef-131">id</span></span>|<span data-ttu-id="49eef-132">String</span><span class="sxs-lookup"><span data-stu-id="49eef-132">String</span></span>|<span data-ttu-id="49eef-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49eef-133">Key of the entity.</span></span>|
|<span data-ttu-id="49eef-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="49eef-134">ruleName</span></span>|<span data-ttu-id="49eef-135">String</span><span class="sxs-lookup"><span data-stu-id="49eef-135">String</span></span>|<span data-ttu-id="49eef-136">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="49eef-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="49eef-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="49eef-137">Response</span></span>
<span data-ttu-id="49eef-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49eef-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49eef-139">Пример</span><span class="sxs-lookup"><span data-stu-id="49eef-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="49eef-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="49eef-140">Request</span></span>
<span data-ttu-id="49eef-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49eef-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="49eef-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="49eef-142">Response</span></span>
<span data-ttu-id="49eef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="49eef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



