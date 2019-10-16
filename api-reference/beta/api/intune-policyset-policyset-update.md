---
title: действие обновления
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94e46588c0c68abefc03a144f5c2edc43350e870
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536324"
---
# <a name="update-action"></a><span data-ttu-id="4a325-103">действие обновления</span><span class="sxs-lookup"><span data-stu-id="4a325-103">update action</span></span>

> <span data-ttu-id="4a325-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a325-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a325-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a325-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4a325-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a325-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4a325-107">Prerequisites</span></span>
<span data-ttu-id="4a325-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a325-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a325-110">Permission type</span></span>|<span data-ttu-id="4a325-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a325-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a325-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a325-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a325-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a325-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a325-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a325-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a325-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a325-115">Not supported.</span></span>|
|<span data-ttu-id="4a325-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a325-116">Application</span></span>|<span data-ttu-id="4a325-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a325-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a325-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a325-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="4a325-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a325-119">Request headers</span></span>
|<span data-ttu-id="4a325-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a325-120">Header</span></span>|<span data-ttu-id="4a325-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a325-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a325-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a325-122">Authorization</span></span>|<span data-ttu-id="4a325-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a325-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a325-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4a325-124">Accept</span></span>|<span data-ttu-id="4a325-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a325-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a325-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a325-126">Request body</span></span>
<span data-ttu-id="4a325-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a325-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4a325-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4a325-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4a325-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a325-129">Property</span></span>|<span data-ttu-id="4a325-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4a325-130">Type</span></span>|<span data-ttu-id="4a325-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4a325-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a325-132">аддедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="4a325-132">addedPolicySetItems</span></span>|<span data-ttu-id="4a325-133">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4a325-133">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="4a325-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4a325-134">Not yet documented</span></span>|
|<span data-ttu-id="4a325-135">упдатедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="4a325-135">updatedPolicySetItems</span></span>|<span data-ttu-id="4a325-136">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4a325-136">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="4a325-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4a325-137">Not yet documented</span></span>|
|<span data-ttu-id="4a325-138">делетедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="4a325-138">deletedPolicySetItems</span></span>|<span data-ttu-id="4a325-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a325-139">String collection</span></span>|<span data-ttu-id="4a325-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4a325-140">Not yet documented</span></span>|
|<span data-ttu-id="4a325-141">assignments</span><span class="sxs-lookup"><span data-stu-id="4a325-141">assignments</span></span>|<span data-ttu-id="4a325-142">Коллекция [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4a325-142">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="4a325-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4a325-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4a325-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a325-144">Response</span></span>
<span data-ttu-id="4a325-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4a325-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4a325-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4a325-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a325-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a325-147">Request</span></span>
<span data-ttu-id="4a325-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a325-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1529

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
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4a325-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a325-149">Response</span></span>
<span data-ttu-id="4a325-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a325-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






