---
title: Обновление Граупполициконфигуратион
description: Обновление свойств объекта Граупполициконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07c13ca22db02707d9aa1ebc63085f0b824cb2b8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355306"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="aa9d6-103">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="aa9d6-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="aa9d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa9d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa9d6-106">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aa9d6-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa9d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aa9d6-107">Prerequisites</span></span>
<span data-ttu-id="aa9d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa9d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa9d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa9d6-110">Permission type</span></span>|<span data-ttu-id="aa9d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa9d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa9d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa9d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa9d6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa9d6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa9d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa9d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa9d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-115">Not supported.</span></span>|
|<span data-ttu-id="aa9d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa9d6-116">Application</span></span>|<span data-ttu-id="aa9d6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa9d6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa9d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa9d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa9d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa9d6-119">Request headers</span></span>
|<span data-ttu-id="aa9d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa9d6-120">Header</span></span>|<span data-ttu-id="aa9d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aa9d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa9d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa9d6-122">Authorization</span></span>|<span data-ttu-id="aa9d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa9d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aa9d6-124">Accept</span></span>|<span data-ttu-id="aa9d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa9d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa9d6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa9d6-126">Request body</span></span>
<span data-ttu-id="aa9d6-127">В тексте запроса добавьте представление объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="aa9d6-128">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa9d6-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="aa9d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa9d6-129">Property</span></span>|<span data-ttu-id="aa9d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aa9d6-130">Type</span></span>|<span data-ttu-id="aa9d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aa9d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa9d6-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa9d6-132">createdDateTime</span></span>|<span data-ttu-id="aa9d6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa9d6-133">DateTimeOffset</span></span>|<span data-ttu-id="aa9d6-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="aa9d6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aa9d6-135">displayName</span></span>|<span data-ttu-id="aa9d6-136">Строка</span><span class="sxs-lookup"><span data-stu-id="aa9d6-136">String</span></span>|<span data-ttu-id="aa9d6-137">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="aa9d6-138">description</span><span class="sxs-lookup"><span data-stu-id="aa9d6-138">description</span></span>|<span data-ttu-id="aa9d6-139">String</span><span class="sxs-lookup"><span data-stu-id="aa9d6-139">String</span></span>|<span data-ttu-id="aa9d6-140">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="aa9d6-141">id</span><span class="sxs-lookup"><span data-stu-id="aa9d6-141">id</span></span>|<span data-ttu-id="aa9d6-142">String</span><span class="sxs-lookup"><span data-stu-id="aa9d6-142">String</span></span>|<span data-ttu-id="aa9d6-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-143">Key of the entity.</span></span>|
|<span data-ttu-id="aa9d6-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa9d6-144">lastModifiedDateTime</span></span>|<span data-ttu-id="aa9d6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa9d6-145">DateTimeOffset</span></span>|<span data-ttu-id="aa9d6-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="aa9d6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa9d6-147">Response</span></span>
<span data-ttu-id="aa9d6-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa9d6-149">Пример</span><span class="sxs-lookup"><span data-stu-id="aa9d6-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa9d6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa9d6-150">Request</span></span>
<span data-ttu-id="aa9d6-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa9d6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa9d6-152">Response</span></span>
<span data-ttu-id="aa9d6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa9d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






