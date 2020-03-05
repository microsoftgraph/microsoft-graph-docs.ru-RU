---
title: Действие createInstance
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6054320e441184d731b82fa287ad1e444f9d7751
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470422"
---
# <a name="createinstance-action"></a><span data-ttu-id="0b339-103">Действие createInstance</span><span class="sxs-lookup"><span data-stu-id="0b339-103">createInstance action</span></span>

<span data-ttu-id="0b339-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0b339-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b339-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b339-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b339-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b339-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b339-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b339-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b339-108">Prerequisites</span></span>
<span data-ttu-id="0b339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b339-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b339-111">Permission type</span></span>|<span data-ttu-id="0b339-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b339-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b339-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b339-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b339-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b339-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b339-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b339-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b339-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b339-116">Not supported.</span></span>|
|<span data-ttu-id="0b339-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b339-117">Application</span></span>|<span data-ttu-id="0b339-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b339-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b339-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b339-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="0b339-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0b339-120">Request headers</span></span>
|<span data-ttu-id="0b339-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b339-121">Header</span></span>|<span data-ttu-id="0b339-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b339-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b339-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b339-123">Authorization</span></span>|<span data-ttu-id="0b339-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b339-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b339-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b339-125">Accept</span></span>|<span data-ttu-id="0b339-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b339-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b339-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b339-127">Request body</span></span>
<span data-ttu-id="0b339-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b339-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0b339-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0b339-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0b339-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b339-130">Property</span></span>|<span data-ttu-id="0b339-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b339-131">Type</span></span>|<span data-ttu-id="0b339-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b339-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b339-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0b339-133">displayName</span></span>|<span data-ttu-id="0b339-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0b339-134">String</span></span>|<span data-ttu-id="0b339-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b339-135">Not yet documented</span></span>|
|<span data-ttu-id="0b339-136">description</span><span class="sxs-lookup"><span data-stu-id="0b339-136">description</span></span>|<span data-ttu-id="0b339-137">String</span><span class="sxs-lookup"><span data-stu-id="0b339-137">String</span></span>|<span data-ttu-id="0b339-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b339-138">Not yet documented</span></span>|
|<span data-ttu-id="0b339-139">сеттингсделта</span><span class="sxs-lookup"><span data-stu-id="0b339-139">settingsDelta</span></span>|<span data-ttu-id="0b339-140">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0b339-140">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="0b339-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b339-141">Not yet documented</span></span>|
|<span data-ttu-id="0b339-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b339-142">roleScopeTagIds</span></span>|<span data-ttu-id="0b339-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0b339-143">String collection</span></span>|<span data-ttu-id="0b339-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0b339-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0b339-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b339-145">Response</span></span>
<span data-ttu-id="0b339-146">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b339-146">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b339-147">Пример</span><span class="sxs-lookup"><span data-stu-id="0b339-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b339-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b339-148">Request</span></span>
<span data-ttu-id="0b339-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b339-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b339-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b339-150">Response</span></span>
<span data-ttu-id="0b339-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b339-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





