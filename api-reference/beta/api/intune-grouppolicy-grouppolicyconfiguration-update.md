---
title: Update groupPolicyConfiguration
description: Обновление свойств объекта groupPolicyConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 294bf20454e597f95d607b04abcdfaa6bd3d4a25
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153400"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="e3f3c-103">Update groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e3f3c-103">Update groupPolicyConfiguration</span></span>

<span data-ttu-id="e3f3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3f3c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3f3c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3f3c-107">Обновление свойств объекта [groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3f3c-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3f3c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3f3c-108">Prerequisites</span></span>
<span data-ttu-id="e3f3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3f3c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3f3c-111">Permission type</span></span>|<span data-ttu-id="e3f3c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3f3c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3f3c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3f3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3f3c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f3c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3f3c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3f3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3f3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-116">Not supported.</span></span>|
|<span data-ttu-id="e3f3c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e3f3c-117">Application</span></span>|<span data-ttu-id="e3f3c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f3c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3f3c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3f3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e3f3c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3f3c-120">Request headers</span></span>
|<span data-ttu-id="e3f3c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3f3c-121">Header</span></span>|<span data-ttu-id="e3f3c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3f3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3f3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3f3c-123">Authorization</span></span>|<span data-ttu-id="e3f3c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3f3c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3f3c-125">Accept</span></span>|<span data-ttu-id="e3f3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3f3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3f3c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3f3c-127">Request body</span></span>
<span data-ttu-id="e3f3c-128">В теле запроса поставляем представление JSON для [объекта GroupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3f3c-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="e3f3c-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3f3c-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="e3f3c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3f3c-130">Property</span></span>|<span data-ttu-id="e3f3c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3f3c-131">Type</span></span>|<span data-ttu-id="e3f3c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3f3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f3c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3f3c-133">createdDateTime</span></span>|<span data-ttu-id="e3f3c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3f3c-134">DateTimeOffset</span></span>|<span data-ttu-id="e3f3c-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="e3f3c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e3f3c-136">displayName</span></span>|<span data-ttu-id="e3f3c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e3f3c-137">String</span></span>|<span data-ttu-id="e3f3c-138">Пользователь предоставил имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="e3f3c-139">description</span><span class="sxs-lookup"><span data-stu-id="e3f3c-139">description</span></span>|<span data-ttu-id="e3f3c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e3f3c-140">String</span></span>|<span data-ttu-id="e3f3c-141">Пользователь предоставил описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="e3f3c-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e3f3c-142">roleScopeTagIds</span></span>|<span data-ttu-id="e3f3c-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e3f3c-143">String collection</span></span>|<span data-ttu-id="e3f3c-144">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="e3f3c-145">id</span><span class="sxs-lookup"><span data-stu-id="e3f3c-145">id</span></span>|<span data-ttu-id="e3f3c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="e3f3c-146">String</span></span>|<span data-ttu-id="e3f3c-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-147">Key of the entity.</span></span>|
|<span data-ttu-id="e3f3c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3f3c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e3f3c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3f3c-149">DateTimeOffset</span></span>|<span data-ttu-id="e3f3c-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e3f3c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3f3c-151">Response</span></span>
<span data-ttu-id="e3f3c-152">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3f3c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e3f3c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3f3c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3f3c-154">Request</span></span>
<span data-ttu-id="e3f3c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3f3c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3f3c-156">Response</span></span>
<span data-ttu-id="e3f3c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3f3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




