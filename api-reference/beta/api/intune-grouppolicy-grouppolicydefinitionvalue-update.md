---
title: Обновление Граупполицидефинитионвалуе
description: Обновление свойств объекта Граупполицидефинитионвалуе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 411e707f9ae7f949f01c605b72210ecef79dbc26
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905079"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="15dac-103">Обновление Граупполицидефинитионвалуе</span><span class="sxs-lookup"><span data-stu-id="15dac-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="15dac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15dac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15dac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15dac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15dac-106">Обновление свойств объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="15dac-106">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15dac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15dac-107">Prerequisites</span></span>
<span data-ttu-id="15dac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15dac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15dac-110">Permission type</span></span>|<span data-ttu-id="15dac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15dac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15dac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15dac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15dac-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15dac-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15dac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15dac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15dac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15dac-115">Not supported.</span></span>|
|<span data-ttu-id="15dac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15dac-116">Application</span></span>|<span data-ttu-id="15dac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15dac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15dac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15dac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="15dac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15dac-119">Request headers</span></span>
|<span data-ttu-id="15dac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15dac-120">Header</span></span>|<span data-ttu-id="15dac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="15dac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15dac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15dac-122">Authorization</span></span>|<span data-ttu-id="15dac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15dac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15dac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15dac-124">Accept</span></span>|<span data-ttu-id="15dac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15dac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15dac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15dac-126">Request body</span></span>
<span data-ttu-id="15dac-127">В тексте запроса добавьте представление объекта [Граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15dac-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="15dac-128">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="15dac-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="15dac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="15dac-129">Property</span></span>|<span data-ttu-id="15dac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15dac-130">Type</span></span>|<span data-ttu-id="15dac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15dac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15dac-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15dac-132">createdDateTime</span></span>|<span data-ttu-id="15dac-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15dac-133">DateTimeOffset</span></span>|<span data-ttu-id="15dac-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="15dac-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="15dac-135">enabled</span><span class="sxs-lookup"><span data-stu-id="15dac-135">enabled</span></span>|<span data-ttu-id="15dac-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="15dac-136">Boolean</span></span>|<span data-ttu-id="15dac-137">Включает или отключает соответствующее определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="15dac-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="15dac-138">Конфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="15dac-138">configurationType</span></span>|[<span data-ttu-id="15dac-139">Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="15dac-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="15dac-140">Указывает, как должно настраиваться значение.</span><span class="sxs-lookup"><span data-stu-id="15dac-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="15dac-141">Это может быть либо политика, либо предпочтение.</span><span class="sxs-lookup"><span data-stu-id="15dac-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="15dac-142">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="15dac-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="15dac-143">id</span><span class="sxs-lookup"><span data-stu-id="15dac-143">id</span></span>|<span data-ttu-id="15dac-144">Строка</span><span class="sxs-lookup"><span data-stu-id="15dac-144">String</span></span>|<span data-ttu-id="15dac-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15dac-145">Key of the entity.</span></span>|
|<span data-ttu-id="15dac-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15dac-146">lastModifiedDateTime</span></span>|<span data-ttu-id="15dac-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15dac-147">DateTimeOffset</span></span>|<span data-ttu-id="15dac-148">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="15dac-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="15dac-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="15dac-149">Response</span></span>
<span data-ttu-id="15dac-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15dac-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15dac-151">Пример</span><span class="sxs-lookup"><span data-stu-id="15dac-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="15dac-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="15dac-152">Request</span></span>
<span data-ttu-id="15dac-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15dac-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="15dac-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="15dac-154">Response</span></span>
<span data-ttu-id="15dac-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15dac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




