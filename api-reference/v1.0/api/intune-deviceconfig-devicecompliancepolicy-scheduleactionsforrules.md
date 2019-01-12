---
title: Действие scheduleActionsForRules
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b7f38e87316b0640b98a97cfbd038ae230832c78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949187"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="62e4d-103">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="62e4d-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="62e4d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62e4d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62e4d-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="62e4d-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62e4d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="62e4d-106">Prerequisites</span></span>
<span data-ttu-id="62e4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62e4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62e4d-109">Permission type</span></span>|<span data-ttu-id="62e4d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62e4d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62e4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62e4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="62e4d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62e4d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62e4d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62e4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62e4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62e4d-114">Not supported.</span></span>|
|<span data-ttu-id="62e4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62e4d-115">Application</span></span>|<span data-ttu-id="62e4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62e4d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62e4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62e4d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="62e4d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62e4d-118">Request headers</span></span>
|<span data-ttu-id="62e4d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62e4d-119">Header</span></span>|<span data-ttu-id="62e4d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="62e4d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62e4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62e4d-121">Authorization</span></span>|<span data-ttu-id="62e4d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62e4d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62e4d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="62e4d-123">Accept</span></span>|<span data-ttu-id="62e4d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="62e4d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62e4d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62e4d-125">Request body</span></span>
<span data-ttu-id="62e4d-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62e4d-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="62e4d-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="62e4d-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="62e4d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="62e4d-128">Property</span></span>|<span data-ttu-id="62e4d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="62e4d-129">Type</span></span>|<span data-ttu-id="62e4d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="62e4d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62e4d-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="62e4d-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="62e4d-132">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="62e4d-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="62e4d-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="62e4d-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="62e4d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="62e4d-134">Response</span></span>
<span data-ttu-id="62e4d-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="62e4d-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="62e4d-136">Пример</span><span class="sxs-lookup"><span data-stu-id="62e4d-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="62e4d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="62e4d-137">Request</span></span>
<span data-ttu-id="62e4d-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62e4d-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="62e4d-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="62e4d-139">Response</span></span>
<span data-ttu-id="62e4d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="62e4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



