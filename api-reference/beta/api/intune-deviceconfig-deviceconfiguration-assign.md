---
title: Действие assign
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d30818be0733d7b571f0c2e32fb01af5570d65
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400335"
---
# <a name="assign-action"></a><span data-ttu-id="f7da9-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="f7da9-103">assign action</span></span>

> <span data-ttu-id="f7da9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7da9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7da9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7da9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7da9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7da9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7da9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7da9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7da9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7da9-108">Prerequisites</span></span>
<span data-ttu-id="f7da9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7da9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7da9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7da9-111">Permission type</span></span>|<span data-ttu-id="f7da9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7da9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7da9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7da9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7da9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7da9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7da9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7da9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7da9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7da9-116">Not supported.</span></span>|
|<span data-ttu-id="f7da9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7da9-117">Application</span></span>|<span data-ttu-id="f7da9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7da9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7da9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7da9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f7da9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7da9-120">Request headers</span></span>
|<span data-ttu-id="f7da9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7da9-121">Header</span></span>|<span data-ttu-id="f7da9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7da9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7da9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7da9-123">Authorization</span></span>|<span data-ttu-id="f7da9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7da9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7da9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7da9-125">Accept</span></span>|<span data-ttu-id="f7da9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7da9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7da9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7da9-127">Request body</span></span>
<span data-ttu-id="f7da9-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7da9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f7da9-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f7da9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f7da9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7da9-130">Property</span></span>|<span data-ttu-id="f7da9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7da9-131">Type</span></span>|<span data-ttu-id="f7da9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7da9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7da9-133">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="f7da9-133">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="f7da9-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f7da9-134">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="f7da9-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7da9-135">Not yet documented</span></span>|
|<span data-ttu-id="f7da9-136">assignments</span><span class="sxs-lookup"><span data-stu-id="f7da9-136">assignments</span></span>|<span data-ttu-id="f7da9-137">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f7da9-137">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f7da9-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7da9-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7da9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7da9-139">Response</span></span>
<span data-ttu-id="f7da9-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7da9-140">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7da9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f7da9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7da9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7da9-142">Request</span></span>
<span data-ttu-id="f7da9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7da9-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7da9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7da9-144">Response</span></span>
<span data-ttu-id="f7da9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7da9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




