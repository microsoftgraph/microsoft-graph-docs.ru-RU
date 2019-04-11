---
title: Создание Граупполицидефинитионвалуе
description: Создание нового объекта Граупполицидефинитионвалуе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fef42cc86aa2cdef23b81223b1e715027c659a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793240"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="23cbb-103">Создание Граупполицидефинитионвалуе</span><span class="sxs-lookup"><span data-stu-id="23cbb-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="23cbb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23cbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23cbb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23cbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23cbb-106">Создание нового объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="23cbb-106">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23cbb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23cbb-107">Prerequisites</span></span>
<span data-ttu-id="23cbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23cbb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23cbb-110">Permission type</span></span>|<span data-ttu-id="23cbb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23cbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23cbb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23cbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23cbb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23cbb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23cbb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23cbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cbb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23cbb-115">Not supported.</span></span>|
|<span data-ttu-id="23cbb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23cbb-116">Application</span></span>|<span data-ttu-id="23cbb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23cbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cbb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23cbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="23cbb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23cbb-119">Request headers</span></span>
|<span data-ttu-id="23cbb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23cbb-120">Header</span></span>|<span data-ttu-id="23cbb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="23cbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23cbb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23cbb-122">Authorization</span></span>|<span data-ttu-id="23cbb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23cbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23cbb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="23cbb-124">Accept</span></span>|<span data-ttu-id="23cbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23cbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23cbb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23cbb-126">Request body</span></span>
<span data-ttu-id="23cbb-127">В тексте запроса добавьте представление объекта Граупполицидефинитионвалуе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23cbb-127">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="23cbb-128">В следующей таблице приведены свойства, необходимые при создании Граупполицидефинитионвалуе.</span><span class="sxs-lookup"><span data-stu-id="23cbb-128">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="23cbb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="23cbb-129">Property</span></span>|<span data-ttu-id="23cbb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="23cbb-130">Type</span></span>|<span data-ttu-id="23cbb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="23cbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23cbb-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23cbb-132">createdDateTime</span></span>|<span data-ttu-id="23cbb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23cbb-133">DateTimeOffset</span></span>|<span data-ttu-id="23cbb-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="23cbb-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="23cbb-135">enabled</span><span class="sxs-lookup"><span data-stu-id="23cbb-135">enabled</span></span>|<span data-ttu-id="23cbb-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="23cbb-136">Boolean</span></span>|<span data-ttu-id="23cbb-137">Включает или отключает соответствующее определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="23cbb-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="23cbb-138">Конфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="23cbb-138">configurationType</span></span>|[<span data-ttu-id="23cbb-139">Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="23cbb-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="23cbb-140">Указывает, как должно настраиваться значение.</span><span class="sxs-lookup"><span data-stu-id="23cbb-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="23cbb-141">Это может быть либо политика, либо предпочтение.</span><span class="sxs-lookup"><span data-stu-id="23cbb-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="23cbb-142">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="23cbb-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="23cbb-143">id</span><span class="sxs-lookup"><span data-stu-id="23cbb-143">id</span></span>|<span data-ttu-id="23cbb-144">String</span><span class="sxs-lookup"><span data-stu-id="23cbb-144">String</span></span>|<span data-ttu-id="23cbb-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="23cbb-145">Key of the entity.</span></span>|
|<span data-ttu-id="23cbb-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23cbb-146">lastModifiedDateTime</span></span>|<span data-ttu-id="23cbb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23cbb-147">DateTimeOffset</span></span>|<span data-ttu-id="23cbb-148">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="23cbb-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="23cbb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="23cbb-149">Response</span></span>
<span data-ttu-id="23cbb-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23cbb-150">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23cbb-151">Пример</span><span class="sxs-lookup"><span data-stu-id="23cbb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="23cbb-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="23cbb-152">Request</span></span>
<span data-ttu-id="23cbb-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23cbb-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23cbb-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="23cbb-154">Response</span></span>
<span data-ttu-id="23cbb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23cbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





