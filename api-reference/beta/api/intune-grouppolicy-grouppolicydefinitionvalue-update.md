---
title: Update groupPolicyDefinitionValue
description: Обновление свойств объекта groupPolicyDefinitionValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb9185810155eace790304a2324ab7bba515cf12
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157494"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="391fc-103">Update groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="391fc-103">Update groupPolicyDefinitionValue</span></span>

<span data-ttu-id="391fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="391fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="391fc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="391fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="391fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="391fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="391fc-107">Обновление свойств объекта [groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="391fc-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="391fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="391fc-108">Prerequisites</span></span>
<span data-ttu-id="391fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="391fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="391fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="391fc-111">Permission type</span></span>|<span data-ttu-id="391fc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="391fc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="391fc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="391fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="391fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="391fc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="391fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="391fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="391fc-116">Not supported.</span></span>|
|<span data-ttu-id="391fc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="391fc-117">Application</span></span>|<span data-ttu-id="391fc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391fc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="391fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="391fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="391fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="391fc-120">Request headers</span></span>
|<span data-ttu-id="391fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="391fc-121">Header</span></span>|<span data-ttu-id="391fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="391fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="391fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="391fc-123">Authorization</span></span>|<span data-ttu-id="391fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="391fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="391fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="391fc-125">Accept</span></span>|<span data-ttu-id="391fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="391fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="391fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="391fc-127">Request body</span></span>
<span data-ttu-id="391fc-128">В теле запроса поставляем представление JSON для [объекта GroupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="391fc-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="391fc-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="391fc-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="391fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="391fc-130">Property</span></span>|<span data-ttu-id="391fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="391fc-131">Type</span></span>|<span data-ttu-id="391fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="391fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="391fc-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="391fc-133">createdDateTime</span></span>|<span data-ttu-id="391fc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="391fc-134">DateTimeOffset</span></span>|<span data-ttu-id="391fc-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="391fc-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="391fc-136">enabled</span><span class="sxs-lookup"><span data-stu-id="391fc-136">enabled</span></span>|<span data-ttu-id="391fc-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="391fc-137">Boolean</span></span>|<span data-ttu-id="391fc-138">Включает или отключает связанное определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="391fc-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="391fc-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="391fc-139">configurationType</span></span>|[<span data-ttu-id="391fc-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="391fc-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="391fc-141">Указывает, как следует настроить значение.</span><span class="sxs-lookup"><span data-stu-id="391fc-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="391fc-142">Это может быть как политика, так и как предпочтение.</span><span class="sxs-lookup"><span data-stu-id="391fc-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="391fc-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="391fc-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="391fc-144">id</span><span class="sxs-lookup"><span data-stu-id="391fc-144">id</span></span>|<span data-ttu-id="391fc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="391fc-145">String</span></span>|<span data-ttu-id="391fc-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="391fc-146">Key of the entity.</span></span>|
|<span data-ttu-id="391fc-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="391fc-147">lastModifiedDateTime</span></span>|<span data-ttu-id="391fc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="391fc-148">DateTimeOffset</span></span>|<span data-ttu-id="391fc-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="391fc-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="391fc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="391fc-150">Response</span></span>
<span data-ttu-id="391fc-151">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="391fc-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="391fc-152">Пример</span><span class="sxs-lookup"><span data-stu-id="391fc-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="391fc-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="391fc-153">Request</span></span>
<span data-ttu-id="391fc-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="391fc-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="391fc-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="391fc-155">Response</span></span>
<span data-ttu-id="391fc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="391fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




