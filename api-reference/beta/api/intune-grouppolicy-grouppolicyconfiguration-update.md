---
title: Обновление Граупполициконфигуратион
description: Обновление свойств объекта Граупполициконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 867d70f3978db683cb154b9e5405df08b315b4b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160034"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="93699-103">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="93699-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="93699-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93699-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93699-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93699-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93699-106">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="93699-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93699-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93699-107">Prerequisites</span></span>
<span data-ttu-id="93699-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93699-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93699-110">Permission type</span></span>|<span data-ttu-id="93699-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93699-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93699-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93699-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93699-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93699-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93699-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93699-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93699-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93699-115">Not supported.</span></span>|
|<span data-ttu-id="93699-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93699-116">Application</span></span>|<span data-ttu-id="93699-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93699-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93699-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93699-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="93699-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93699-119">Request headers</span></span>
|<span data-ttu-id="93699-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93699-120">Header</span></span>|<span data-ttu-id="93699-121">Значение</span><span class="sxs-lookup"><span data-stu-id="93699-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93699-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93699-122">Authorization</span></span>|<span data-ttu-id="93699-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="93699-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93699-124">Accept</span><span class="sxs-lookup"><span data-stu-id="93699-124">Accept</span></span>|<span data-ttu-id="93699-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93699-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93699-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93699-126">Request body</span></span>
<span data-ttu-id="93699-127">В тексте запроса добавьте представление объекта [Граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93699-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="93699-128">В следующей таблице приведены свойства, необходимые при создании [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="93699-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="93699-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="93699-129">Property</span></span>|<span data-ttu-id="93699-130">Тип</span><span class="sxs-lookup"><span data-stu-id="93699-130">Type</span></span>|<span data-ttu-id="93699-131">Описание</span><span class="sxs-lookup"><span data-stu-id="93699-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93699-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93699-132">createdDateTime</span></span>|<span data-ttu-id="93699-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93699-133">DateTimeOffset</span></span>|<span data-ttu-id="93699-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="93699-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="93699-135">displayName</span><span class="sxs-lookup"><span data-stu-id="93699-135">displayName</span></span>|<span data-ttu-id="93699-136">String</span><span class="sxs-lookup"><span data-stu-id="93699-136">String</span></span>|<span data-ttu-id="93699-137">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="93699-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="93699-138">description</span><span class="sxs-lookup"><span data-stu-id="93699-138">description</span></span>|<span data-ttu-id="93699-139">String</span><span class="sxs-lookup"><span data-stu-id="93699-139">String</span></span>|<span data-ttu-id="93699-140">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="93699-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="93699-141">id</span><span class="sxs-lookup"><span data-stu-id="93699-141">id</span></span>|<span data-ttu-id="93699-142">String</span><span class="sxs-lookup"><span data-stu-id="93699-142">String</span></span>|<span data-ttu-id="93699-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="93699-143">Key of the entity.</span></span>|
|<span data-ttu-id="93699-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93699-144">lastModifiedDateTime</span></span>|<span data-ttu-id="93699-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93699-145">DateTimeOffset</span></span>|<span data-ttu-id="93699-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="93699-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="93699-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="93699-147">Response</span></span>
<span data-ttu-id="93699-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93699-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93699-149">Пример</span><span class="sxs-lookup"><span data-stu-id="93699-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="93699-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="93699-150">Request</span></span>
<span data-ttu-id="93699-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93699-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93699-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="93699-152">Response</span></span>
<span data-ttu-id="93699-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93699-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




