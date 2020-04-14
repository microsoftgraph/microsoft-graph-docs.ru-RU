---
title: Создание Граупполицидефинитионвалуе
description: Создание нового объекта Граупполицидефинитионвалуе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8327d26dc2966f141a5c76e1b419101c130c88be
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454518"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="b1af7-103">Создание Граупполицидефинитионвалуе</span><span class="sxs-lookup"><span data-stu-id="b1af7-103">Create groupPolicyDefinitionValue</span></span>

<span data-ttu-id="b1af7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1af7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1af7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1af7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1af7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1af7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1af7-107">Создание нового объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="b1af7-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1af7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1af7-108">Prerequisites</span></span>
<span data-ttu-id="b1af7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1af7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1af7-111">Permission type</span></span>|<span data-ttu-id="b1af7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1af7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1af7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1af7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1af7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1af7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1af7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1af7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1af7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1af7-116">Not supported.</span></span>|
|<span data-ttu-id="b1af7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1af7-117">Application</span></span>|<span data-ttu-id="b1af7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1af7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1af7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1af7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="b1af7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1af7-120">Request headers</span></span>
|<span data-ttu-id="b1af7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1af7-121">Header</span></span>|<span data-ttu-id="b1af7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1af7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1af7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1af7-123">Authorization</span></span>|<span data-ttu-id="b1af7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1af7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1af7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1af7-125">Accept</span></span>|<span data-ttu-id="b1af7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1af7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1af7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1af7-127">Request body</span></span>
<span data-ttu-id="b1af7-128">В тексте запроса добавьте представление объекта Граупполицидефинитионвалуе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1af7-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="b1af7-129">В следующей таблице приведены свойства, необходимые при создании Граупполицидефинитионвалуе.</span><span class="sxs-lookup"><span data-stu-id="b1af7-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="b1af7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1af7-130">Property</span></span>|<span data-ttu-id="b1af7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1af7-131">Type</span></span>|<span data-ttu-id="b1af7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1af7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1af7-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1af7-133">createdDateTime</span></span>|<span data-ttu-id="b1af7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1af7-134">DateTimeOffset</span></span>|<span data-ttu-id="b1af7-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b1af7-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="b1af7-136">enabled</span><span class="sxs-lookup"><span data-stu-id="b1af7-136">enabled</span></span>|<span data-ttu-id="b1af7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1af7-137">Boolean</span></span>|<span data-ttu-id="b1af7-138">Включает или отключает соответствующее определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="b1af7-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="b1af7-139">конфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="b1af7-139">configurationType</span></span>|[<span data-ttu-id="b1af7-140">граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="b1af7-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="b1af7-141">Указывает, как должно настраиваться значение.</span><span class="sxs-lookup"><span data-stu-id="b1af7-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="b1af7-142">Это может быть либо политика, либо предпочтение.</span><span class="sxs-lookup"><span data-stu-id="b1af7-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="b1af7-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="b1af7-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="b1af7-144">id</span><span class="sxs-lookup"><span data-stu-id="b1af7-144">id</span></span>|<span data-ttu-id="b1af7-145">String</span><span class="sxs-lookup"><span data-stu-id="b1af7-145">String</span></span>|<span data-ttu-id="b1af7-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1af7-146">Key of the entity.</span></span>|
|<span data-ttu-id="b1af7-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1af7-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b1af7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1af7-148">DateTimeOffset</span></span>|<span data-ttu-id="b1af7-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b1af7-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b1af7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1af7-150">Response</span></span>
<span data-ttu-id="b1af7-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1af7-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1af7-152">Пример</span><span class="sxs-lookup"><span data-stu-id="b1af7-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1af7-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1af7-153">Request</span></span>
<span data-ttu-id="b1af7-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1af7-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="b1af7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1af7-155">Response</span></span>
<span data-ttu-id="b1af7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1af7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



