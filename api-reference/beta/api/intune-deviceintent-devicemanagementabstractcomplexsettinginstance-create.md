---
title: Создание Девицеманажементабстракткомплекссеттингинстанце
description: Создание нового объекта Девицеманажементабстракткомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d20f2a65db92823fd8e10bb261d3469d45fa12b9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732256"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="44a6b-103">Создание Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="44a6b-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="44a6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44a6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44a6b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44a6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44a6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44a6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44a6b-107">Создание нового объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="44a6b-107">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44a6b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44a6b-108">Prerequisites</span></span>
<span data-ttu-id="44a6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44a6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44a6b-111">Permission type</span></span>|<span data-ttu-id="44a6b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44a6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44a6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44a6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44a6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44a6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44a6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44a6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44a6b-116">Not supported.</span></span>|
|<span data-ttu-id="44a6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44a6b-117">Application</span></span>|<span data-ttu-id="44a6b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a6b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44a6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44a6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="44a6b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44a6b-120">Request headers</span></span>
|<span data-ttu-id="44a6b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44a6b-121">Header</span></span>|<span data-ttu-id="44a6b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44a6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44a6b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44a6b-123">Authorization</span></span>|<span data-ttu-id="44a6b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44a6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44a6b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44a6b-125">Accept</span></span>|<span data-ttu-id="44a6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44a6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44a6b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44a6b-127">Request body</span></span>
<span data-ttu-id="44a6b-128">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44a6b-128">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="44a6b-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="44a6b-129">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="44a6b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44a6b-130">Property</span></span>|<span data-ttu-id="44a6b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44a6b-131">Type</span></span>|<span data-ttu-id="44a6b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44a6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44a6b-133">id</span><span class="sxs-lookup"><span data-stu-id="44a6b-133">id</span></span>|<span data-ttu-id="44a6b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="44a6b-134">String</span></span>|<span data-ttu-id="44a6b-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="44a6b-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="44a6b-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="44a6b-136">definitionId</span></span>|<span data-ttu-id="44a6b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="44a6b-137">String</span></span>|<span data-ttu-id="44a6b-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="44a6b-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="44a6b-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="44a6b-139">valueJson</span></span>|<span data-ttu-id="44a6b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="44a6b-140">String</span></span>|<span data-ttu-id="44a6b-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="44a6b-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="44a6b-142">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="44a6b-142">implementationId</span></span>|<span data-ttu-id="44a6b-143">Строка</span><span class="sxs-lookup"><span data-stu-id="44a6b-143">String</span></span>|<span data-ttu-id="44a6b-144">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="44a6b-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="44a6b-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="44a6b-145">Response</span></span>
<span data-ttu-id="44a6b-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44a6b-146">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44a6b-147">Пример</span><span class="sxs-lookup"><span data-stu-id="44a6b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="44a6b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="44a6b-148">Request</span></span>
<span data-ttu-id="44a6b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44a6b-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="44a6b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="44a6b-150">Response</span></span>
<span data-ttu-id="44a6b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44a6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```





