---
title: Создание Девицеманажементабстракткомплекссеттингинстанце
description: Создание нового объекта Девицеманажементабстракткомплекссеттингинстанце.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 754ea0cfa4b8c79f77b4cc22731d3b3b341e266b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510698"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="d7683-103">Создание Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="d7683-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="d7683-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7683-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7683-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7683-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7683-106">Создание нового объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="d7683-106">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7683-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7683-107">Prerequisites</span></span>
<span data-ttu-id="d7683-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7683-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7683-110">Permission type</span></span>|<span data-ttu-id="d7683-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7683-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7683-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7683-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7683-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7683-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7683-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7683-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7683-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7683-115">Not supported.</span></span>|
|<span data-ttu-id="d7683-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7683-116">Application</span></span>|<span data-ttu-id="d7683-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7683-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7683-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7683-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d7683-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7683-119">Request headers</span></span>
|<span data-ttu-id="d7683-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7683-120">Header</span></span>|<span data-ttu-id="d7683-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7683-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7683-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7683-122">Authorization</span></span>|<span data-ttu-id="d7683-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7683-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7683-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d7683-124">Accept</span></span>|<span data-ttu-id="d7683-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7683-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7683-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7683-126">Request body</span></span>
<span data-ttu-id="d7683-127">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7683-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="d7683-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="d7683-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="d7683-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7683-129">Property</span></span>|<span data-ttu-id="d7683-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d7683-130">Type</span></span>|<span data-ttu-id="d7683-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d7683-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7683-132">id</span><span class="sxs-lookup"><span data-stu-id="d7683-132">id</span></span>|<span data-ttu-id="d7683-133">String</span><span class="sxs-lookup"><span data-stu-id="d7683-133">String</span></span>|<span data-ttu-id="d7683-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d7683-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d7683-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="d7683-135">definitionId</span></span>|<span data-ttu-id="d7683-136">String</span><span class="sxs-lookup"><span data-stu-id="d7683-136">String</span></span>|<span data-ttu-id="d7683-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d7683-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d7683-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="d7683-138">valueJson</span></span>|<span data-ttu-id="d7683-139">String</span><span class="sxs-lookup"><span data-stu-id="d7683-139">String</span></span>|<span data-ttu-id="d7683-140">Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d7683-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d7683-141">Имплементатионид</span><span class="sxs-lookup"><span data-stu-id="d7683-141">implementationId</span></span>|<span data-ttu-id="d7683-142">String</span><span class="sxs-lookup"><span data-stu-id="d7683-142">String</span></span>|<span data-ttu-id="d7683-143">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="d7683-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="d7683-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7683-144">Response</span></span>
<span data-ttu-id="d7683-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7683-145">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7683-146">Пример</span><span class="sxs-lookup"><span data-stu-id="d7683-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7683-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7683-147">Request</span></span>
<span data-ttu-id="d7683-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7683-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7683-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7683-149">Response</span></span>
<span data-ttu-id="d7683-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7683-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





