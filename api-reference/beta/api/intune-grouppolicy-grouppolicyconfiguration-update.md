---
title: Обновление Граупполициконфигуратион
description: Обновление свойств объекта Граупполициконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c44cada3024c3d1ec5818fc21d0301951cd581ab
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724201"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="3e4ba-103">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3e4ba-103">Update groupPolicyConfiguration</span></span>

<span data-ttu-id="3e4ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e4ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e4ba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e4ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e4ba-107">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3e4ba-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e4ba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e4ba-108">Prerequisites</span></span>
<span data-ttu-id="3e4ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e4ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4ba-111">Permission type</span></span>|<span data-ttu-id="3e4ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e4ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e4ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e4ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e4ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e4ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e4ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e4ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-116">Not supported.</span></span>|
|<span data-ttu-id="3e4ba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e4ba-117">Application</span></span>|<span data-ttu-id="3e4ba-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4ba-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e4ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e4ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3e4ba-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e4ba-120">Request headers</span></span>
|<span data-ttu-id="3e4ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e4ba-121">Header</span></span>|<span data-ttu-id="3e4ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e4ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e4ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e4ba-123">Authorization</span></span>|<span data-ttu-id="3e4ba-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e4ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e4ba-125">Accept</span></span>|<span data-ttu-id="3e4ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e4ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4ba-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e4ba-127">Request body</span></span>
<span data-ttu-id="3e4ba-128">В тексте запроса добавьте представление объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="3e4ba-129">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e4ba-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="3e4ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e4ba-130">Property</span></span>|<span data-ttu-id="3e4ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3e4ba-131">Type</span></span>|<span data-ttu-id="3e4ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3e4ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e4ba-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4ba-133">createdDateTime</span></span>|<span data-ttu-id="3e4ba-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4ba-134">DateTimeOffset</span></span>|<span data-ttu-id="3e4ba-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="3e4ba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3e4ba-136">displayName</span></span>|<span data-ttu-id="3e4ba-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4ba-137">String</span></span>|<span data-ttu-id="3e4ba-138">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="3e4ba-139">description</span><span class="sxs-lookup"><span data-stu-id="3e4ba-139">description</span></span>|<span data-ttu-id="3e4ba-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4ba-140">String</span></span>|<span data-ttu-id="3e4ba-141">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="3e4ba-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e4ba-142">roleScopeTagIds</span></span>|<span data-ttu-id="3e4ba-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e4ba-143">String collection</span></span>|<span data-ttu-id="3e4ba-144">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="3e4ba-145">id</span><span class="sxs-lookup"><span data-stu-id="3e4ba-145">id</span></span>|<span data-ttu-id="3e4ba-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4ba-146">String</span></span>|<span data-ttu-id="3e4ba-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-147">Key of the entity.</span></span>|
|<span data-ttu-id="3e4ba-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4ba-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3e4ba-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4ba-149">DateTimeOffset</span></span>|<span data-ttu-id="3e4ba-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3e4ba-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e4ba-151">Response</span></span>
<span data-ttu-id="3e4ba-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4ba-153">Пример</span><span class="sxs-lookup"><span data-stu-id="3e4ba-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e4ba-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e4ba-154">Request</span></span>
<span data-ttu-id="3e4ba-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e4ba-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e4ba-156">Response</span></span>
<span data-ttu-id="3e4ba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e4ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





