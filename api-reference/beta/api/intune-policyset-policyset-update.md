---
title: действие обновления
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09004e387725a0a537fc6a1f2560f19af67e4e7b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940947"
---
# <a name="update-action"></a><span data-ttu-id="41807-103">действие обновления</span><span class="sxs-lookup"><span data-stu-id="41807-103">update action</span></span>

> <span data-ttu-id="41807-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41807-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41807-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41807-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41807-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="41807-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41807-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41807-107">Prerequisites</span></span>
<span data-ttu-id="41807-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41807-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41807-110">Permission type</span></span>|<span data-ttu-id="41807-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41807-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41807-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41807-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41807-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41807-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41807-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41807-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41807-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41807-115">Not supported.</span></span>|
|<span data-ttu-id="41807-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41807-116">Application</span></span>|<span data-ttu-id="41807-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41807-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41807-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41807-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="41807-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="41807-119">Request headers</span></span>
|<span data-ttu-id="41807-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41807-120">Header</span></span>|<span data-ttu-id="41807-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41807-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41807-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41807-122">Authorization</span></span>|<span data-ttu-id="41807-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41807-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41807-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41807-124">Accept</span></span>|<span data-ttu-id="41807-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41807-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41807-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41807-126">Request body</span></span>
<span data-ttu-id="41807-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41807-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="41807-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="41807-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="41807-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="41807-129">Property</span></span>|<span data-ttu-id="41807-130">Тип</span><span class="sxs-lookup"><span data-stu-id="41807-130">Type</span></span>|<span data-ttu-id="41807-131">Описание</span><span class="sxs-lookup"><span data-stu-id="41807-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41807-132">аддедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="41807-132">addedPolicySetItems</span></span>|<span data-ttu-id="41807-133">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="41807-133">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="41807-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="41807-134">Not yet documented</span></span>|
|<span data-ttu-id="41807-135">упдатедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="41807-135">updatedPolicySetItems</span></span>|<span data-ttu-id="41807-136">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="41807-136">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="41807-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="41807-137">Not yet documented</span></span>|
|<span data-ttu-id="41807-138">делетедполицисетитемс</span><span class="sxs-lookup"><span data-stu-id="41807-138">deletedPolicySetItems</span></span>|<span data-ttu-id="41807-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="41807-139">String collection</span></span>|<span data-ttu-id="41807-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="41807-140">Not yet documented</span></span>|
|<span data-ttu-id="41807-141">assignments</span><span class="sxs-lookup"><span data-stu-id="41807-141">assignments</span></span>|<span data-ttu-id="41807-142">Коллекция [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41807-142">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="41807-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="41807-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="41807-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="41807-144">Response</span></span>
<span data-ttu-id="41807-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="41807-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41807-146">Пример</span><span class="sxs-lookup"><span data-stu-id="41807-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="41807-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="41807-147">Request</span></span>
<span data-ttu-id="41807-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41807-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41807-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="41807-149">Response</span></span>
<span data-ttu-id="41807-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41807-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





