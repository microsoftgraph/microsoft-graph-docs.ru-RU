---
title: Действие scheduleActionsForRules
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f01770280fe5c1d588d4cfeb5b9ce240fb0dfe16
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940098"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="02a0b-103">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="02a0b-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="02a0b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02a0b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02a0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02a0b-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="02a0b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02a0b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="02a0b-107">Prerequisites</span></span>
<span data-ttu-id="02a0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02a0b-110">Permission type</span></span>|<span data-ttu-id="02a0b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02a0b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02a0b-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="02a0b-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="02a0b-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="02a0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02a0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02a0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a0b-116">Not supported.</span></span>|
|<span data-ttu-id="02a0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02a0b-117">Application</span></span>||
| <span data-ttu-id="02a0b-118">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="02a0b-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="02a0b-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a0b-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a0b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02a0b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="02a0b-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02a0b-121">Request headers</span></span>
|<span data-ttu-id="02a0b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02a0b-122">Header</span></span>|<span data-ttu-id="02a0b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="02a0b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a0b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02a0b-124">Authorization</span></span>|<span data-ttu-id="02a0b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02a0b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02a0b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="02a0b-126">Accept</span></span>|<span data-ttu-id="02a0b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="02a0b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a0b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02a0b-128">Request body</span></span>
<span data-ttu-id="02a0b-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02a0b-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="02a0b-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="02a0b-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="02a0b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="02a0b-131">Property</span></span>|<span data-ttu-id="02a0b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="02a0b-132">Type</span></span>|<span data-ttu-id="02a0b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="02a0b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a0b-134">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="02a0b-134">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="02a0b-135">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="02a0b-135">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="02a0b-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="02a0b-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="02a0b-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="02a0b-137">Response</span></span>
<span data-ttu-id="02a0b-138">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02a0b-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02a0b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="02a0b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="02a0b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="02a0b-140">Request</span></span>
<span data-ttu-id="02a0b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02a0b-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02a0b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="02a0b-142">Response</span></span>
<span data-ttu-id="02a0b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02a0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








