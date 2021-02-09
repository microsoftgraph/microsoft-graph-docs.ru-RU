---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b078d917482bc1d62c51f9e1d3d9008d94d8432f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156569"
---
# <a name="assign-action"></a><span data-ttu-id="efd36-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="efd36-103">assign action</span></span>

<span data-ttu-id="efd36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efd36-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efd36-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efd36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd36-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="efd36-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efd36-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="efd36-108">Prerequisites</span></span>
<span data-ttu-id="efd36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efd36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efd36-111">Permission type</span></span>|<span data-ttu-id="efd36-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efd36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efd36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efd36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efd36-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd36-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efd36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efd36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efd36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd36-116">Not supported.</span></span>|
|<span data-ttu-id="efd36-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efd36-117">Application</span></span>|<span data-ttu-id="efd36-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd36-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efd36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efd36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="efd36-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efd36-120">Request headers</span></span>
|<span data-ttu-id="efd36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efd36-121">Header</span></span>|<span data-ttu-id="efd36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="efd36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efd36-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efd36-123">Authorization</span></span>|<span data-ttu-id="efd36-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efd36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efd36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efd36-125">Accept</span></span>|<span data-ttu-id="efd36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efd36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd36-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efd36-127">Request body</span></span>
<span data-ttu-id="efd36-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efd36-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="efd36-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="efd36-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="efd36-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="efd36-130">Property</span></span>|<span data-ttu-id="efd36-131">Тип</span><span class="sxs-lookup"><span data-stu-id="efd36-131">Type</span></span>|<span data-ttu-id="efd36-132">Описание</span><span class="sxs-lookup"><span data-stu-id="efd36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd36-133">assignments</span><span class="sxs-lookup"><span data-stu-id="efd36-133">assignments</span></span>|<span data-ttu-id="efd36-134">[Коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="efd36-134">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="efd36-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="efd36-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="efd36-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="efd36-136">Response</span></span>
<span data-ttu-id="efd36-137">В случае успешного выполнения это действие возвращает код отклика и коллекцию `200 OK` [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efd36-137">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd36-138">Пример</span><span class="sxs-lookup"><span data-stu-id="efd36-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="efd36-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="efd36-139">Request</span></span>
<span data-ttu-id="efd36-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efd36-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign

Content-type: application/json
Content-length: 524

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="efd36-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="efd36-141">Response</span></span>
<span data-ttu-id="efd36-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efd36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




