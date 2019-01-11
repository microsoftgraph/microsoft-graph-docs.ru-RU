---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 540037998280858e50cf1ee6a9996664ff45d1c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836976"
---
# <a name="assign-action"></a><span data-ttu-id="0e9e2-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="0e9e2-103">assign action</span></span>

> <span data-ttu-id="0e9e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e9e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e9e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e9e2-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0e9e2-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e9e2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0e9e2-108">Prerequisites</span></span>
<span data-ttu-id="0e9e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e9e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e9e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e9e2-111">Permission type</span></span>|<span data-ttu-id="0e9e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e9e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e9e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e9e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e9e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e9e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e9e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e9e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e9e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-116">Not supported.</span></span>|
|<span data-ttu-id="0e9e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e9e2-117">Application</span></span>|<span data-ttu-id="0e9e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e9e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e9e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0e9e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e9e2-120">Request headers</span></span>
|<span data-ttu-id="0e9e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e9e2-121">Header</span></span>|<span data-ttu-id="0e9e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e9e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e9e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e9e2-123">Authorization</span></span>|<span data-ttu-id="0e9e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e9e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e9e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e9e2-125">Accept</span></span>|<span data-ttu-id="0e9e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e9e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e9e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e9e2-127">Request body</span></span>
<span data-ttu-id="0e9e2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0e9e2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0e9e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e9e2-130">Property</span></span>|<span data-ttu-id="0e9e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0e9e2-131">Type</span></span>|<span data-ttu-id="0e9e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0e9e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e9e2-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="0e9e2-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="0e9e2-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0e9e2-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0e9e2-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0e9e2-135">Not yet documented</span></span>|
|<span data-ttu-id="0e9e2-136">assignments</span><span class="sxs-lookup"><span data-stu-id="0e9e2-136">assignments</span></span>|<span data-ttu-id="0e9e2-137">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0e9e2-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0e9e2-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0e9e2-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0e9e2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e9e2-139">Response</span></span>
<span data-ttu-id="0e9e2-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e9e2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0e9e2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e9e2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e9e2-142">Request</span></span>
<span data-ttu-id="0e9e2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0e9e2-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e9e2-144">Response</span></span>
<span data-ttu-id="0e9e2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e9e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





