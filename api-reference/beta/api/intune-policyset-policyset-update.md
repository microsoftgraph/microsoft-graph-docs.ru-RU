---
title: действие обновления
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 406c27f5e57c0aa4ac68e66ab53d1bdd77b9811b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791723"
---
# <a name="update-action"></a><span data-ttu-id="d706a-103">действие обновления</span><span class="sxs-lookup"><span data-stu-id="d706a-103">update action</span></span>

<span data-ttu-id="d706a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d706a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d706a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d706a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d706a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d706a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d706a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d706a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d706a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d706a-108">Prerequisites</span></span>
<span data-ttu-id="d706a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d706a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d706a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d706a-111">Permission type</span></span>|<span data-ttu-id="d706a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d706a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d706a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d706a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d706a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d706a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d706a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d706a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d706a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d706a-116">Not supported.</span></span>|
|<span data-ttu-id="d706a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d706a-117">Application</span></span>|<span data-ttu-id="d706a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d706a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d706a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d706a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="d706a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d706a-120">Request headers</span></span>
|<span data-ttu-id="d706a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d706a-121">Header</span></span>|<span data-ttu-id="d706a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d706a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d706a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d706a-123">Authorization</span></span>|<span data-ttu-id="d706a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d706a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d706a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d706a-125">Accept</span></span>|<span data-ttu-id="d706a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d706a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d706a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d706a-127">Request body</span></span>
<span data-ttu-id="d706a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d706a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d706a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d706a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d706a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d706a-130">Property</span></span>|<span data-ttu-id="d706a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d706a-131">Type</span></span>|<span data-ttu-id="d706a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d706a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d706a-133">аддедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="d706a-133">addedPolicySetItems</span></span>|<span data-ttu-id="d706a-134">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d706a-134">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="d706a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d706a-135">Not yet documented</span></span>|
|<span data-ttu-id="d706a-136">упдатедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="d706a-136">updatedPolicySetItems</span></span>|<span data-ttu-id="d706a-137">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="d706a-137">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="d706a-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d706a-138">Not yet documented</span></span>|
|<span data-ttu-id="d706a-139">делетедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="d706a-139">deletedPolicySetItems</span></span>|<span data-ttu-id="d706a-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d706a-140">String collection</span></span>|<span data-ttu-id="d706a-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d706a-141">Not yet documented</span></span>|
|<span data-ttu-id="d706a-142">assignments</span><span class="sxs-lookup"><span data-stu-id="d706a-142">assignments</span></span>|<span data-ttu-id="d706a-143">Коллекция [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d706a-143">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="d706a-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d706a-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d706a-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="d706a-145">Response</span></span>
<span data-ttu-id="d706a-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d706a-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d706a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d706a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d706a-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d706a-148">Request</span></span>
<span data-ttu-id="d706a-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d706a-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1692

{
  "addedPolicySetItems": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ],
  "updatedPolicySetItems": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ],
  "deletedPolicySetItems": [
    "Deleted Policy Set Items value"
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.policySetAssignment",
      "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d706a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d706a-150">Response</span></span>
<span data-ttu-id="d706a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d706a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



