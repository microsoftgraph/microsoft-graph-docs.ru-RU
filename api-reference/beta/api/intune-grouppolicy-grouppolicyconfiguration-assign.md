---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8182bb0f7c335602966903c4540135ef0d75dfa8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465319"
---
# <a name="assign-action"></a><span data-ttu-id="e3c0d-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="e3c0d-103">assign action</span></span>

<span data-ttu-id="e3c0d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e3c0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3c0d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3c0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3c0d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3c0d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e3c0d-108">Prerequisites</span></span>
<span data-ttu-id="e3c0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c0d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3c0d-111">Permission type</span></span>|<span data-ttu-id="e3c0d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3c0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3c0d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3c0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3c0d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c0d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e3c0d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3c0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3c0d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-116">Not supported.</span></span>|
|<span data-ttu-id="e3c0d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3c0d-117">Application</span></span>|<span data-ttu-id="e3c0d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c0d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3c0d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3c0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e3c0d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3c0d-120">Request headers</span></span>
|<span data-ttu-id="e3c0d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3c0d-121">Header</span></span>|<span data-ttu-id="e3c0d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3c0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3c0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3c0d-123">Authorization</span></span>|<span data-ttu-id="e3c0d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3c0d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3c0d-125">Accept</span></span>|<span data-ttu-id="e3c0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3c0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c0d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3c0d-127">Request body</span></span>
<span data-ttu-id="e3c0d-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e3c0d-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e3c0d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3c0d-130">Property</span></span>|<span data-ttu-id="e3c0d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3c0d-131">Type</span></span>|<span data-ttu-id="e3c0d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3c0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c0d-133">assignments</span><span class="sxs-lookup"><span data-stu-id="e3c0d-133">assignments</span></span>|<span data-ttu-id="e3c0d-134">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e3c0d-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e3c0d-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e3c0d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e3c0d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3c0d-136">Response</span></span>
<span data-ttu-id="e3c0d-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3c0d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e3c0d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3c0d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3c0d-139">Request</span></span>
<span data-ttu-id="e3c0d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e3c0d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3c0d-141">Response</span></span>
<span data-ttu-id="e3c0d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3c0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





