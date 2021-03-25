---
title: Создание groupPolicyConfiguration
description: Создайте новый объект groupPolicyConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0964d6eac276d42292e4417e9bfbb0e643101597
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153470"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="49492-103">Создание groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="49492-103">Create groupPolicyConfiguration</span></span>

<span data-ttu-id="49492-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49492-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49492-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49492-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49492-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49492-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49492-107">Создайте новый [объект groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49492-107">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49492-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49492-108">Prerequisites</span></span>
<span data-ttu-id="49492-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49492-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49492-111">Permission type</span></span>|<span data-ttu-id="49492-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49492-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49492-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49492-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49492-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49492-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49492-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49492-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49492-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49492-116">Not supported.</span></span>|
|<span data-ttu-id="49492-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="49492-117">Application</span></span>|<span data-ttu-id="49492-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49492-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49492-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49492-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49492-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49492-120">Request headers</span></span>
|<span data-ttu-id="49492-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49492-121">Header</span></span>|<span data-ttu-id="49492-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49492-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49492-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49492-123">Authorization</span></span>|<span data-ttu-id="49492-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49492-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49492-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49492-125">Accept</span></span>|<span data-ttu-id="49492-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49492-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49492-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49492-127">Request body</span></span>
<span data-ttu-id="49492-128">В теле запроса поставляем представление JSON для объекта GroupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49492-128">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="49492-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49492-129">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="49492-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49492-130">Property</span></span>|<span data-ttu-id="49492-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49492-131">Type</span></span>|<span data-ttu-id="49492-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49492-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49492-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49492-133">createdDateTime</span></span>|<span data-ttu-id="49492-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49492-134">DateTimeOffset</span></span>|<span data-ttu-id="49492-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="49492-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="49492-136">displayName</span><span class="sxs-lookup"><span data-stu-id="49492-136">displayName</span></span>|<span data-ttu-id="49492-137">Строка</span><span class="sxs-lookup"><span data-stu-id="49492-137">String</span></span>|<span data-ttu-id="49492-138">Пользователь предоставил имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="49492-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="49492-139">description</span><span class="sxs-lookup"><span data-stu-id="49492-139">description</span></span>|<span data-ttu-id="49492-140">Строка</span><span class="sxs-lookup"><span data-stu-id="49492-140">String</span></span>|<span data-ttu-id="49492-141">Пользователь предоставил описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="49492-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="49492-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49492-142">roleScopeTagIds</span></span>|<span data-ttu-id="49492-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49492-143">String collection</span></span>|<span data-ttu-id="49492-144">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="49492-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="49492-145">id</span><span class="sxs-lookup"><span data-stu-id="49492-145">id</span></span>|<span data-ttu-id="49492-146">Строка</span><span class="sxs-lookup"><span data-stu-id="49492-146">String</span></span>|<span data-ttu-id="49492-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49492-147">Key of the entity.</span></span>|
|<span data-ttu-id="49492-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49492-148">lastModifiedDateTime</span></span>|<span data-ttu-id="49492-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49492-149">DateTimeOffset</span></span>|<span data-ttu-id="49492-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="49492-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="49492-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="49492-151">Response</span></span>
<span data-ttu-id="49492-152">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49492-152">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49492-153">Пример</span><span class="sxs-lookup"><span data-stu-id="49492-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="49492-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="49492-154">Request</span></span>
<span data-ttu-id="49492-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49492-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
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

### <a name="response"></a><span data-ttu-id="49492-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="49492-156">Response</span></span>
<span data-ttu-id="49492-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49492-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




