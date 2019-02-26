---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b423e5b16b130e348862a91f0af84b307a3b768c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144697"
---
# <a name="assign-action"></a><span data-ttu-id="b2c5f-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="b2c5f-103">assign action</span></span>

> <span data-ttu-id="b2c5f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2c5f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c5f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2c5f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2c5f-107">Prerequisites</span></span>
<span data-ttu-id="b2c5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2c5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2c5f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2c5f-110">Permission type</span></span>|<span data-ttu-id="b2c5f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2c5f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2c5f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2c5f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2c5f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2c5f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2c5f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2c5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2c5f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-115">Not supported.</span></span>|
|<span data-ttu-id="b2c5f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2c5f-116">Application</span></span>|<span data-ttu-id="b2c5f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2c5f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2c5f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b2c5f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2c5f-119">Request headers</span></span>
|<span data-ttu-id="b2c5f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2c5f-120">Header</span></span>|<span data-ttu-id="b2c5f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2c5f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2c5f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2c5f-122">Authorization</span></span>|<span data-ttu-id="b2c5f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2c5f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2c5f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2c5f-124">Accept</span></span>|<span data-ttu-id="b2c5f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2c5f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2c5f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2c5f-126">Request body</span></span>
<span data-ttu-id="b2c5f-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b2c5f-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b2c5f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2c5f-129">Property</span></span>|<span data-ttu-id="b2c5f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b2c5f-130">Type</span></span>|<span data-ttu-id="b2c5f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b2c5f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c5f-132">Девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="b2c5f-132">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="b2c5f-133">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2c5f-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="b2c5f-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2c5f-134">Not yet documented</span></span>|
|<span data-ttu-id="b2c5f-135">assignments</span><span class="sxs-lookup"><span data-stu-id="b2c5f-135">assignments</span></span>|<span data-ttu-id="b2c5f-136">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2c5f-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b2c5f-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2c5f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b2c5f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2c5f-138">Response</span></span>
<span data-ttu-id="b2c5f-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2c5f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b2c5f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2c5f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2c5f-141">Request</span></span>
<span data-ttu-id="b2c5f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2c5f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2c5f-143">Response</span></span>
<span data-ttu-id="b2c5f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2c5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




