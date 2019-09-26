---
title: Обновление Граупполициконфигуратион
description: Обновление свойств объекта Граупполициконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d8251112cb2c5e84345deeeebd5504c6e0fc4e6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184201"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="37476-103">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="37476-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="37476-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37476-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37476-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37476-106">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="37476-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37476-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37476-107">Prerequisites</span></span>
<span data-ttu-id="37476-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37476-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37476-110">Permission type</span></span>|<span data-ttu-id="37476-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37476-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37476-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37476-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37476-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37476-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="37476-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37476-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37476-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37476-115">Not supported.</span></span>|
|<span data-ttu-id="37476-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37476-116">Application</span></span>|<span data-ttu-id="37476-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37476-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37476-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37476-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="37476-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37476-119">Request headers</span></span>
|<span data-ttu-id="37476-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37476-120">Header</span></span>|<span data-ttu-id="37476-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37476-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37476-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37476-122">Authorization</span></span>|<span data-ttu-id="37476-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37476-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37476-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37476-124">Accept</span></span>|<span data-ttu-id="37476-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37476-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37476-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37476-126">Request body</span></span>
<span data-ttu-id="37476-127">В тексте запроса добавьте представление объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37476-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="37476-128">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37476-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="37476-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37476-129">Property</span></span>|<span data-ttu-id="37476-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37476-130">Type</span></span>|<span data-ttu-id="37476-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37476-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37476-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37476-132">createdDateTime</span></span>|<span data-ttu-id="37476-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37476-133">DateTimeOffset</span></span>|<span data-ttu-id="37476-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="37476-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="37476-135">displayName</span><span class="sxs-lookup"><span data-stu-id="37476-135">displayName</span></span>|<span data-ttu-id="37476-136">Строка</span><span class="sxs-lookup"><span data-stu-id="37476-136">String</span></span>|<span data-ttu-id="37476-137">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="37476-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="37476-138">description</span><span class="sxs-lookup"><span data-stu-id="37476-138">description</span></span>|<span data-ttu-id="37476-139">String</span><span class="sxs-lookup"><span data-stu-id="37476-139">String</span></span>|<span data-ttu-id="37476-140">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="37476-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="37476-141">id</span><span class="sxs-lookup"><span data-stu-id="37476-141">id</span></span>|<span data-ttu-id="37476-142">String</span><span class="sxs-lookup"><span data-stu-id="37476-142">String</span></span>|<span data-ttu-id="37476-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37476-143">Key of the entity.</span></span>|
|<span data-ttu-id="37476-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37476-144">lastModifiedDateTime</span></span>|<span data-ttu-id="37476-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37476-145">DateTimeOffset</span></span>|<span data-ttu-id="37476-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="37476-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="37476-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="37476-147">Response</span></span>
<span data-ttu-id="37476-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37476-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37476-149">Пример</span><span class="sxs-lookup"><span data-stu-id="37476-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="37476-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="37476-150">Request</span></span>
<span data-ttu-id="37476-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37476-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="37476-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="37476-152">Response</span></span>
<span data-ttu-id="37476-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37476-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




