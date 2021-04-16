---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f21c1bfca18b433dbd05d2aa855db7ed3aafbec
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867149"
---
# <a name="assign-action"></a><span data-ttu-id="b2681-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="b2681-103">assign action</span></span>

<span data-ttu-id="b2681-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2681-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2681-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2681-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2681-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2681-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2681-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b2681-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2681-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2681-108">Prerequisites</span></span>
<span data-ttu-id="b2681-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2681-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2681-111">Permission type</span></span>|<span data-ttu-id="b2681-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2681-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2681-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2681-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2681-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2681-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2681-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2681-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2681-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2681-116">Not supported.</span></span>|
|<span data-ttu-id="b2681-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b2681-117">Application</span></span>|<span data-ttu-id="b2681-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2681-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2681-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2681-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b2681-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2681-120">Request headers</span></span>
|<span data-ttu-id="b2681-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2681-121">Header</span></span>|<span data-ttu-id="b2681-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2681-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2681-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2681-123">Authorization</span></span>|<span data-ttu-id="b2681-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2681-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2681-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2681-125">Accept</span></span>|<span data-ttu-id="b2681-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2681-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2681-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2681-127">Request body</span></span>
<span data-ttu-id="b2681-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2681-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b2681-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b2681-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b2681-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2681-130">Property</span></span>|<span data-ttu-id="b2681-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b2681-131">Type</span></span>|<span data-ttu-id="b2681-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b2681-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2681-133">assignments</span><span class="sxs-lookup"><span data-stu-id="b2681-133">assignments</span></span>|<span data-ttu-id="b2681-134">[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2681-134">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="b2681-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b2681-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b2681-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2681-136">Response</span></span>
<span data-ttu-id="b2681-137">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [коллекцию deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b2681-137">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2681-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b2681-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2681-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2681-139">Request</span></span>
<span data-ttu-id="b2681-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2681-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2681-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2681-141">Response</span></span>
<span data-ttu-id="b2681-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2681-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




