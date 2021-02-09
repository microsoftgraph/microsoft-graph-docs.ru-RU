---
title: Действие validateComplianceScript
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d590bd85ecd5bfb8d16589c268f88fb593eeb63
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157031"
---
# <a name="validatecompliancescript-action"></a><span data-ttu-id="87572-103">Действие validateComplianceScript</span><span class="sxs-lookup"><span data-stu-id="87572-103">validateComplianceScript action</span></span>

<span data-ttu-id="87572-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87572-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87572-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87572-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87572-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87572-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87572-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="87572-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87572-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="87572-108">Prerequisites</span></span>
<span data-ttu-id="87572-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87572-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87572-111">Permission type</span></span>|<span data-ttu-id="87572-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87572-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87572-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87572-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87572-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87572-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87572-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87572-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87572-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87572-116">Not supported.</span></span>|
|<span data-ttu-id="87572-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87572-117">Application</span></span>|<span data-ttu-id="87572-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87572-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87572-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87572-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/validateComplianceScript
```

## <a name="request-headers"></a><span data-ttu-id="87572-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87572-120">Request headers</span></span>
|<span data-ttu-id="87572-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87572-121">Header</span></span>|<span data-ttu-id="87572-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87572-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87572-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87572-123">Authorization</span></span>|<span data-ttu-id="87572-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87572-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87572-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87572-125">Accept</span></span>|<span data-ttu-id="87572-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87572-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87572-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87572-127">Request body</span></span>
<span data-ttu-id="87572-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87572-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="87572-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="87572-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="87572-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="87572-130">Property</span></span>|<span data-ttu-id="87572-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87572-131">Type</span></span>|<span data-ttu-id="87572-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87572-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87572-133">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="87572-133">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="87572-134">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="87572-134">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="87572-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="87572-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="87572-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="87572-136">Response</span></span>
<span data-ttu-id="87572-137">В случае успеха это действие возвращает код отклика и `200 OK` [deviceComplianceScriptValidationResult](../resources/intune-deviceconfig-devicecompliancescriptvalidationresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87572-137">If successful, this action returns a `200 OK` response code and a [deviceComplianceScriptValidationResult](../resources/intune-deviceconfig-devicecompliancescriptvalidationresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87572-138">Пример</span><span class="sxs-lookup"><span data-stu-id="87572-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="87572-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="87572-139">Request</span></span>
<span data-ttu-id="87572-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87572-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/validateComplianceScript

Content-type: application/json
Content-length: 224

{
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="87572-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="87572-141">Response</span></span>
<span data-ttu-id="87572-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87572-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1045

{
  "value": {
    "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult",
    "rules": [
      {
        "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
        "settingName": "Setting Name value",
        "operator": "and",
        "deviceComplianceScriptRulOperator": "and",
        "dataType": "boolean",
        "deviceComplianceScriptRuleDataType": "boolean",
        "operand": "Operand value"
      }
    ],
    "scriptErrors": [
      {
        "@odata.type": "microsoft.graph.deviceComplianceScriptError",
        "code": "jsonFileInvalid",
        "deviceComplianceScriptRulesValidationError": "jsonFileInvalid",
        "message": "Message value"
      }
    ],
    "ruleErrors": [
      {
        "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
        "code": "jsonFileInvalid",
        "deviceComplianceScriptRulesValidationError": "jsonFileInvalid",
        "message": "Message value",
        "settingName": "Setting Name value"
      }
    ]
  }
}
```




