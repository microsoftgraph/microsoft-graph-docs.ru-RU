---
title: Обновление Граупполициконфигуратион
description: Обновление свойств объекта Граупполициконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc1e0079e86bc480b11f1fe05a1a8cca4c17693e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087084"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="3870a-103">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3870a-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="3870a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3870a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3870a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3870a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3870a-106">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3870a-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3870a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3870a-107">Prerequisites</span></span>
<span data-ttu-id="3870a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3870a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3870a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3870a-110">Permission type</span></span>|<span data-ttu-id="3870a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3870a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3870a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3870a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3870a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3870a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3870a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3870a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3870a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3870a-115">Not supported.</span></span>|
|<span data-ttu-id="3870a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3870a-116">Application</span></span>|<span data-ttu-id="3870a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3870a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3870a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3870a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3870a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3870a-119">Request headers</span></span>
|<span data-ttu-id="3870a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3870a-120">Header</span></span>|<span data-ttu-id="3870a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3870a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3870a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3870a-122">Authorization</span></span>|<span data-ttu-id="3870a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3870a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3870a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3870a-124">Accept</span></span>|<span data-ttu-id="3870a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3870a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3870a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3870a-126">Request body</span></span>
<span data-ttu-id="3870a-127">В тексте запроса добавьте представление объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3870a-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="3870a-128">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3870a-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="3870a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3870a-129">Property</span></span>|<span data-ttu-id="3870a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3870a-130">Type</span></span>|<span data-ttu-id="3870a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3870a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3870a-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3870a-132">createdDateTime</span></span>|<span data-ttu-id="3870a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3870a-133">DateTimeOffset</span></span>|<span data-ttu-id="3870a-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3870a-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="3870a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3870a-135">displayName</span></span>|<span data-ttu-id="3870a-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3870a-136">String</span></span>|<span data-ttu-id="3870a-137">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="3870a-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="3870a-138">description</span><span class="sxs-lookup"><span data-stu-id="3870a-138">description</span></span>|<span data-ttu-id="3870a-139">String</span><span class="sxs-lookup"><span data-stu-id="3870a-139">String</span></span>|<span data-ttu-id="3870a-140">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="3870a-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="3870a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3870a-141">roleScopeTagIds</span></span>|<span data-ttu-id="3870a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3870a-142">String collection</span></span>|<span data-ttu-id="3870a-143">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3870a-143">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="3870a-144">id</span><span class="sxs-lookup"><span data-stu-id="3870a-144">id</span></span>|<span data-ttu-id="3870a-145">String</span><span class="sxs-lookup"><span data-stu-id="3870a-145">String</span></span>|<span data-ttu-id="3870a-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3870a-146">Key of the entity.</span></span>|
|<span data-ttu-id="3870a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3870a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="3870a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3870a-148">DateTimeOffset</span></span>|<span data-ttu-id="3870a-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3870a-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3870a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3870a-150">Response</span></span>
<span data-ttu-id="3870a-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3870a-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3870a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="3870a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3870a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="3870a-153">Request</span></span>
<span data-ttu-id="3870a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3870a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3870a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3870a-155">Response</span></span>
<span data-ttu-id="3870a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3870a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






