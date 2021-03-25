---
title: Действие createInstance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c581094f94c63014b2d5b8ad47f075d8ddd2a3c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150705"
---
# <a name="createinstance-action"></a><span data-ttu-id="daeaf-103">Действие createInstance</span><span class="sxs-lookup"><span data-stu-id="daeaf-103">createInstance action</span></span>

<span data-ttu-id="daeaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daeaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daeaf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daeaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daeaf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daeaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daeaf-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="daeaf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daeaf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="daeaf-108">Prerequisites</span></span>
<span data-ttu-id="daeaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daeaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daeaf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daeaf-111">Permission type</span></span>|<span data-ttu-id="daeaf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="daeaf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daeaf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daeaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="daeaf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daeaf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="daeaf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daeaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daeaf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daeaf-116">Not supported.</span></span>|
|<span data-ttu-id="daeaf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="daeaf-117">Application</span></span>|<span data-ttu-id="daeaf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daeaf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daeaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daeaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="daeaf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="daeaf-120">Request headers</span></span>
|<span data-ttu-id="daeaf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="daeaf-121">Header</span></span>|<span data-ttu-id="daeaf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="daeaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daeaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="daeaf-123">Authorization</span></span>|<span data-ttu-id="daeaf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daeaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daeaf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="daeaf-125">Accept</span></span>|<span data-ttu-id="daeaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="daeaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daeaf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daeaf-127">Request body</span></span>
<span data-ttu-id="daeaf-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daeaf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="daeaf-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="daeaf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="daeaf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="daeaf-130">Property</span></span>|<span data-ttu-id="daeaf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="daeaf-131">Type</span></span>|<span data-ttu-id="daeaf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="daeaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daeaf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="daeaf-133">displayName</span></span>|<span data-ttu-id="daeaf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="daeaf-134">String</span></span>|<span data-ttu-id="daeaf-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="daeaf-135">Not yet documented</span></span>|
|<span data-ttu-id="daeaf-136">description</span><span class="sxs-lookup"><span data-stu-id="daeaf-136">description</span></span>|<span data-ttu-id="daeaf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="daeaf-137">String</span></span>|<span data-ttu-id="daeaf-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="daeaf-138">Not yet documented</span></span>|
|<span data-ttu-id="daeaf-139">settingsDelta</span><span class="sxs-lookup"><span data-stu-id="daeaf-139">settingsDelta</span></span>|<span data-ttu-id="daeaf-140">[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="daeaf-140">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="daeaf-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="daeaf-141">Not yet documented</span></span>|
|<span data-ttu-id="daeaf-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="daeaf-142">roleScopeTagIds</span></span>|<span data-ttu-id="daeaf-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="daeaf-143">String collection</span></span>|<span data-ttu-id="daeaf-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="daeaf-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="daeaf-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="daeaf-145">Response</span></span>
<span data-ttu-id="daeaf-146">В случае успешного выполнения это действие возвращает код отклика и `200 OK` [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="daeaf-146">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daeaf-147">Пример</span><span class="sxs-lookup"><span data-stu-id="daeaf-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="daeaf-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="daeaf-148">Request</span></span>
<span data-ttu-id="daeaf-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daeaf-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 398

{
  "displayName": "Display Name value",
  "description": "Description value",
  "settingsDelta": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="daeaf-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="daeaf-150">Response</span></span>
<span data-ttu-id="daeaf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="daeaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




