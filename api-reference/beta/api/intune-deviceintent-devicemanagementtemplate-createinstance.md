---
title: Действие createInstance
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026cc2175fbb826fd6068adec68a9661215981ab
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959763"
---
# <a name="createinstance-action"></a><span data-ttu-id="7f42e-103">Действие createInstance</span><span class="sxs-lookup"><span data-stu-id="7f42e-103">createInstance action</span></span>

> <span data-ttu-id="7f42e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f42e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f42e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f42e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f42e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f42e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f42e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f42e-107">Prerequisites</span></span>
<span data-ttu-id="7f42e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f42e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f42e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f42e-110">Permission type</span></span>|<span data-ttu-id="7f42e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f42e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f42e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f42e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f42e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f42e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f42e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f42e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f42e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f42e-115">Not supported.</span></span>|
|<span data-ttu-id="7f42e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f42e-116">Application</span></span>|<span data-ttu-id="7f42e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f42e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f42e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f42e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/createInstance
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/createInstance
```

## <a name="request-headers"></a><span data-ttu-id="7f42e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f42e-119">Request headers</span></span>
|<span data-ttu-id="7f42e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f42e-120">Header</span></span>|<span data-ttu-id="7f42e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7f42e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f42e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f42e-122">Authorization</span></span>|<span data-ttu-id="7f42e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f42e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f42e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7f42e-124">Accept</span></span>|<span data-ttu-id="7f42e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f42e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f42e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f42e-126">Request body</span></span>
<span data-ttu-id="7f42e-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f42e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7f42e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7f42e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7f42e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f42e-129">Property</span></span>|<span data-ttu-id="7f42e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f42e-130">Type</span></span>|<span data-ttu-id="7f42e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f42e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f42e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7f42e-132">displayName</span></span>|<span data-ttu-id="7f42e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7f42e-133">String</span></span>|<span data-ttu-id="7f42e-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7f42e-134">Not yet documented</span></span>|
|<span data-ttu-id="7f42e-135">description</span><span class="sxs-lookup"><span data-stu-id="7f42e-135">description</span></span>|<span data-ttu-id="7f42e-136">String</span><span class="sxs-lookup"><span data-stu-id="7f42e-136">String</span></span>|<span data-ttu-id="7f42e-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f42e-137">Not yet documented</span></span>|
|<span data-ttu-id="7f42e-138">Сеттингсделта</span><span class="sxs-lookup"><span data-stu-id="7f42e-138">settingsDelta</span></span>|<span data-ttu-id="7f42e-139">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="7f42e-139">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="7f42e-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7f42e-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7f42e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f42e-141">Response</span></span>
<span data-ttu-id="7f42e-142">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f42e-142">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f42e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="7f42e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f42e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f42e-144">Request</span></span>
<span data-ttu-id="7f42e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f42e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/createInstance

Content-type: application/json
Content-length: 336

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="7f42e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f42e-146">Response</span></span>
<span data-ttu-id="7f42e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f42e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





