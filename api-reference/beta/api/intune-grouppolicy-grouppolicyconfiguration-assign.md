---
title: Действие assign
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54ba196c8a6b8425bcbfb475247ca67e6675ded8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532179"
---
# <a name="assign-action"></a><span data-ttu-id="7d7f1-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="7d7f1-103">assign action</span></span>

> <span data-ttu-id="7d7f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d7f1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d7f1-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d7f1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d7f1-107">Prerequisites</span></span>
<span data-ttu-id="7d7f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d7f1-110">Permission type</span></span>|<span data-ttu-id="7d7f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d7f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d7f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d7f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d7f1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7f1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d7f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d7f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d7f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-115">Not supported.</span></span>|
|<span data-ttu-id="7d7f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d7f1-116">Application</span></span>|<span data-ttu-id="7d7f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d7f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d7f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7d7f1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d7f1-119">Request headers</span></span>
|<span data-ttu-id="7d7f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d7f1-120">Header</span></span>|<span data-ttu-id="7d7f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7d7f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d7f1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d7f1-122">Authorization</span></span>|<span data-ttu-id="7d7f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d7f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7d7f1-124">Accept</span></span>|<span data-ttu-id="7d7f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d7f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7f1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d7f1-126">Request body</span></span>
<span data-ttu-id="7d7f1-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7d7f1-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7d7f1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d7f1-129">Property</span></span>|<span data-ttu-id="7d7f1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7d7f1-130">Type</span></span>|<span data-ttu-id="7d7f1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7d7f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7f1-132">assignments</span><span class="sxs-lookup"><span data-stu-id="7d7f1-132">assignments</span></span>|<span data-ttu-id="7d7f1-133">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d7f1-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7d7f1-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7d7f1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7d7f1-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d7f1-135">Response</span></span>
<span data-ttu-id="7d7f1-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-136">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7f1-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7d7f1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d7f1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d7f1-138">Request</span></span>
<span data-ttu-id="7d7f1-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d7f1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d7f1-140">Response</span></span>
<span data-ttu-id="7d7f1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d7f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





