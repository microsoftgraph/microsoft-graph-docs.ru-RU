---
title: Действие scheduleActionsForRules
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07af9d9f21891c0ff3547dcb10ca080584bc6617
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801175"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="8cb33-103">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="8cb33-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="8cb33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cb33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cb33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb33-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8cb33-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cb33-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8cb33-107">Prerequisites</span></span>
<span data-ttu-id="8cb33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cb33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cb33-110">Permission type</span></span>|<span data-ttu-id="8cb33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cb33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cb33-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8cb33-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8cb33-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8cb33-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb33-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cb33-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cb33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb33-116">Not supported.</span></span>|
|<span data-ttu-id="8cb33-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8cb33-117">Application</span></span>||
| <span data-ttu-id="8cb33-118">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8cb33-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8cb33-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb33-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb33-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cb33-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="8cb33-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8cb33-121">Request headers</span></span>
|<span data-ttu-id="8cb33-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cb33-122">Header</span></span>|<span data-ttu-id="8cb33-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8cb33-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb33-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb33-124">Authorization</span></span>|<span data-ttu-id="8cb33-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cb33-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb33-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8cb33-126">Accept</span></span>|<span data-ttu-id="8cb33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb33-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb33-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cb33-128">Request body</span></span>
<span data-ttu-id="8cb33-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cb33-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8cb33-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8cb33-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8cb33-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cb33-131">Property</span></span>|<span data-ttu-id="8cb33-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8cb33-132">Type</span></span>|<span data-ttu-id="8cb33-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8cb33-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb33-134">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="8cb33-134">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="8cb33-135">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="8cb33-135">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="8cb33-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8cb33-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8cb33-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cb33-137">Response</span></span>
<span data-ttu-id="8cb33-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8cb33-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8cb33-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8cb33-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cb33-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cb33-140">Request</span></span>
<span data-ttu-id="8cb33-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cb33-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

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

### <a name="response"></a><span data-ttu-id="8cb33-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cb33-142">Response</span></span>
<span data-ttu-id="8cb33-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cb33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







