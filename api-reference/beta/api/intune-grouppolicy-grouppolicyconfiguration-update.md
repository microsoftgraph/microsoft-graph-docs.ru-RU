---
title: Обновление Граупполициконфигуратион
description: Обновление свойств объекта Граупполициконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6265e7b9382322a138c39f05f57daa4579452a82
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804487"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="6f4a8-103">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6f4a8-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="6f4a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f4a8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f4a8-106">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6f4a8-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f4a8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f4a8-107">Prerequisites</span></span>
<span data-ttu-id="6f4a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f4a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f4a8-110">Permission type</span></span>|<span data-ttu-id="6f4a8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f4a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f4a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f4a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f4a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f4a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f4a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f4a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f4a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-115">Not supported.</span></span>|
|<span data-ttu-id="6f4a8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f4a8-116">Application</span></span>|<span data-ttu-id="6f4a8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f4a8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f4a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f4a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f4a8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f4a8-119">Request headers</span></span>
|<span data-ttu-id="6f4a8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f4a8-120">Header</span></span>|<span data-ttu-id="6f4a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6f4a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f4a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f4a8-122">Authorization</span></span>|<span data-ttu-id="6f4a8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f4a8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6f4a8-124">Accept</span></span>|<span data-ttu-id="6f4a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f4a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f4a8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f4a8-126">Request body</span></span>
<span data-ttu-id="6f4a8-127">В тексте запроса добавьте представление объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="6f4a8-128">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f4a8-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="6f4a8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f4a8-129">Property</span></span>|<span data-ttu-id="6f4a8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6f4a8-130">Type</span></span>|<span data-ttu-id="6f4a8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6f4a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f4a8-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f4a8-132">createdDateTime</span></span>|<span data-ttu-id="6f4a8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f4a8-133">DateTimeOffset</span></span>|<span data-ttu-id="6f4a8-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="6f4a8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6f4a8-135">displayName</span></span>|<span data-ttu-id="6f4a8-136">Строка</span><span class="sxs-lookup"><span data-stu-id="6f4a8-136">String</span></span>|<span data-ttu-id="6f4a8-137">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="6f4a8-138">description</span><span class="sxs-lookup"><span data-stu-id="6f4a8-138">description</span></span>|<span data-ttu-id="6f4a8-139">String</span><span class="sxs-lookup"><span data-stu-id="6f4a8-139">String</span></span>|<span data-ttu-id="6f4a8-140">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="6f4a8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f4a8-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f4a8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f4a8-142">String collection</span></span>|<span data-ttu-id="6f4a8-143">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-143">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="6f4a8-144">id</span><span class="sxs-lookup"><span data-stu-id="6f4a8-144">id</span></span>|<span data-ttu-id="6f4a8-145">String</span><span class="sxs-lookup"><span data-stu-id="6f4a8-145">String</span></span>|<span data-ttu-id="6f4a8-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-146">Key of the entity.</span></span>|
|<span data-ttu-id="6f4a8-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f4a8-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6f4a8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f4a8-148">DateTimeOffset</span></span>|<span data-ttu-id="6f4a8-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6f4a8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f4a8-150">Response</span></span>
<span data-ttu-id="6f4a8-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f4a8-152">Пример</span><span class="sxs-lookup"><span data-stu-id="6f4a8-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f4a8-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f4a8-153">Request</span></span>
<span data-ttu-id="6f4a8-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f4a8-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f4a8-155">Response</span></span>
<span data-ttu-id="6f4a8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f4a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




