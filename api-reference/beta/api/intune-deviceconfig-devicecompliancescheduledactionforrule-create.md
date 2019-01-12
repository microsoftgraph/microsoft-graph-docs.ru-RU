---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 217ad13de93f45ce288a39cad766ce2e64dc97cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926612"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="dc7b1-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="dc7b1-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="dc7b1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc7b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc7b1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc7b1-107">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="dc7b1-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc7b1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dc7b1-108">Prerequisites</span></span>
<span data-ttu-id="dc7b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc7b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc7b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc7b1-111">Permission type</span></span>|<span data-ttu-id="dc7b1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc7b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc7b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc7b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc7b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc7b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc7b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc7b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc7b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-116">Not supported.</span></span>|
|<span data-ttu-id="dc7b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc7b1-117">Application</span></span>|<span data-ttu-id="dc7b1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc7b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc7b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="dc7b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc7b1-120">Request headers</span></span>
|<span data-ttu-id="dc7b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc7b1-121">Header</span></span>|<span data-ttu-id="dc7b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc7b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc7b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc7b1-123">Authorization</span></span>|<span data-ttu-id="dc7b1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc7b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc7b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc7b1-125">Accept</span></span>|<span data-ttu-id="dc7b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc7b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc7b1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc7b1-127">Request body</span></span>
<span data-ttu-id="dc7b1-128">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="dc7b1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="dc7b1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc7b1-130">Property</span></span>|<span data-ttu-id="dc7b1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc7b1-131">Type</span></span>|<span data-ttu-id="dc7b1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc7b1-133">id</span><span class="sxs-lookup"><span data-stu-id="dc7b1-133">id</span></span>|<span data-ttu-id="dc7b1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dc7b1-134">String</span></span>|<span data-ttu-id="dc7b1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-135">Key of the entity.</span></span>|
|<span data-ttu-id="dc7b1-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="dc7b1-136">ruleName</span></span>|<span data-ttu-id="dc7b1-137">String</span><span class="sxs-lookup"><span data-stu-id="dc7b1-137">String</span></span>|<span data-ttu-id="dc7b1-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="dc7b1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc7b1-139">Response</span></span>
<span data-ttu-id="dc7b1-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc7b1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dc7b1-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc7b1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc7b1-142">Request</span></span>
<span data-ttu-id="dc7b1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="dc7b1-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc7b1-144">Response</span></span>
<span data-ttu-id="dc7b1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dc7b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





