---
title: Создание Девицеманажементабстракткомплекссеттингинстанце
description: Создание нового объекта Девицеманажементабстракткомплекссеттингинстанце.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78dfa99d046782ed68432268b0c8ad6e58cf8ac8
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522820"
---
# <a name="create-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="d2f94-103">Создание Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="d2f94-103">Create deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="d2f94-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2f94-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2f94-106">Создание нового объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="d2f94-106">Create a new [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2f94-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2f94-107">Prerequisites</span></span>
<span data-ttu-id="d2f94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f94-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f94-110">Permission type</span></span>|<span data-ttu-id="d2f94-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2f94-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2f94-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2f94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f94-115">Not supported.</span></span>|
|<span data-ttu-id="d2f94-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f94-116">Application</span></span>|<span data-ttu-id="d2f94-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2f94-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f94-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d2f94-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f94-119">Request headers</span></span>
|<span data-ttu-id="d2f94-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2f94-120">Header</span></span>|<span data-ttu-id="d2f94-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2f94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2f94-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f94-122">Authorization</span></span>|<span data-ttu-id="d2f94-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2f94-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d2f94-124">Accept</span></span>|<span data-ttu-id="d2f94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2f94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f94-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f94-126">Request body</span></span>
<span data-ttu-id="d2f94-127">В тексте запроса добавьте представление объекта Девицеманажементабстракткомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2f94-127">In the request body, supply a JSON representation for the deviceManagementAbstractComplexSettingInstance object.</span></span>

<span data-ttu-id="d2f94-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементабстракткомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="d2f94-128">The following table shows the properties that are required when you create the deviceManagementAbstractComplexSettingInstance.</span></span>

|<span data-ttu-id="d2f94-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2f94-129">Property</span></span>|<span data-ttu-id="d2f94-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d2f94-130">Type</span></span>|<span data-ttu-id="d2f94-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d2f94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2f94-132">id</span><span class="sxs-lookup"><span data-stu-id="d2f94-132">id</span></span>|<span data-ttu-id="d2f94-133">String</span><span class="sxs-lookup"><span data-stu-id="d2f94-133">String</span></span>|<span data-ttu-id="d2f94-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d2f94-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d2f94-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="d2f94-135">definitionId</span></span>|<span data-ttu-id="d2f94-136">String</span><span class="sxs-lookup"><span data-stu-id="d2f94-136">String</span></span>|<span data-ttu-id="d2f94-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d2f94-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d2f94-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="d2f94-138">valueJson</span></span>|<span data-ttu-id="d2f94-139">String</span><span class="sxs-lookup"><span data-stu-id="d2f94-139">String</span></span>|<span data-ttu-id="d2f94-140">Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d2f94-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d2f94-141">Имплементатионид</span><span class="sxs-lookup"><span data-stu-id="d2f94-141">implementationId</span></span>|<span data-ttu-id="d2f94-142">String</span><span class="sxs-lookup"><span data-stu-id="d2f94-142">String</span></span>|<span data-ttu-id="d2f94-143">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="d2f94-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="d2f94-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f94-144">Response</span></span>
<span data-ttu-id="d2f94-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f94-145">If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f94-146">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f94-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2f94-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f94-147">Request</span></span>
<span data-ttu-id="d2f94-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f94-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2f94-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f94-149">Response</span></span>
<span data-ttu-id="d2f94-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2f94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







