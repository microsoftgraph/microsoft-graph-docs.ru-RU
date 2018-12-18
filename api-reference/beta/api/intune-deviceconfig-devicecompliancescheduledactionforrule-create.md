---
title: Создание объекта deviceComplianceScheduledActionForRule
description: Создание объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
ms.openlocfilehash: adc4e488d387c5f5087ded96e585a882ee424707
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345831"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="8f774-103">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="8f774-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="8f774-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f774-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f774-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f774-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f774-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f774-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f774-107">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="8f774-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f774-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8f774-108">Prerequisites</span></span>
<span data-ttu-id="8f774-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f774-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f774-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f774-111">Permission type</span></span>|<span data-ttu-id="8f774-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f774-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f774-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f774-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f774-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f774-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f774-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f774-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f774-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f774-116">Not supported.</span></span>|
|<span data-ttu-id="8f774-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f774-117">Application</span></span>|<span data-ttu-id="8f774-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f774-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f774-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f774-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="8f774-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f774-120">Request headers</span></span>
|<span data-ttu-id="8f774-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f774-121">Header</span></span>|<span data-ttu-id="8f774-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f774-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f774-123">Authorization</span></span>|<span data-ttu-id="8f774-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f774-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f774-125">Accept</span></span>|<span data-ttu-id="8f774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f774-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f774-127">Request body</span></span>
<span data-ttu-id="8f774-128">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f774-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="8f774-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="8f774-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="8f774-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f774-130">Property</span></span>|<span data-ttu-id="8f774-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f774-131">Type</span></span>|<span data-ttu-id="8f774-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f774-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f774-133">id</span><span class="sxs-lookup"><span data-stu-id="8f774-133">id</span></span>|<span data-ttu-id="8f774-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8f774-134">String</span></span>|<span data-ttu-id="8f774-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f774-135">Key of the entity.</span></span>|
|<span data-ttu-id="8f774-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="8f774-136">ruleName</span></span>|<span data-ttu-id="8f774-137">String</span><span class="sxs-lookup"><span data-stu-id="8f774-137">String</span></span>|<span data-ttu-id="8f774-138">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="8f774-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="8f774-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f774-139">Response</span></span>
<span data-ttu-id="8f774-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f774-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f774-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8f774-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f774-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f774-142">Request</span></span>
<span data-ttu-id="8f774-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f774-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="8f774-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f774-144">Response</span></span>
<span data-ttu-id="8f774-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f774-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





