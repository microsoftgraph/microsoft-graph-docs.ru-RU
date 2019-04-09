---
title: Создание Девицеманажементкомплекссеттингинстанце
description: Создание нового объекта Девицеманажементкомплекссеттингинстанце.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 380f436ffde3720210a1c5cc4084c43d30d9de6b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522792"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="4457c-103">Создание Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="4457c-103">Create deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="4457c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4457c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4457c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4457c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4457c-106">Создание нового объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="4457c-106">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4457c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4457c-107">Prerequisites</span></span>
<span data-ttu-id="4457c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4457c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4457c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4457c-110">Permission type</span></span>|<span data-ttu-id="4457c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4457c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4457c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4457c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4457c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4457c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4457c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4457c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4457c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4457c-115">Not supported.</span></span>|
|<span data-ttu-id="4457c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4457c-116">Application</span></span>|<span data-ttu-id="4457c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4457c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4457c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4457c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4457c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4457c-119">Request headers</span></span>
|<span data-ttu-id="4457c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4457c-120">Header</span></span>|<span data-ttu-id="4457c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4457c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4457c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4457c-122">Authorization</span></span>|<span data-ttu-id="4457c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4457c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4457c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4457c-124">Accept</span></span>|<span data-ttu-id="4457c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4457c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4457c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4457c-126">Request body</span></span>
<span data-ttu-id="4457c-127">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4457c-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="4457c-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="4457c-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="4457c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4457c-129">Property</span></span>|<span data-ttu-id="4457c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4457c-130">Type</span></span>|<span data-ttu-id="4457c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4457c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4457c-132">id</span><span class="sxs-lookup"><span data-stu-id="4457c-132">id</span></span>|<span data-ttu-id="4457c-133">String</span><span class="sxs-lookup"><span data-stu-id="4457c-133">String</span></span>|<span data-ttu-id="4457c-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4457c-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4457c-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="4457c-135">definitionId</span></span>|<span data-ttu-id="4457c-136">String</span><span class="sxs-lookup"><span data-stu-id="4457c-136">String</span></span>|<span data-ttu-id="4457c-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4457c-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4457c-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="4457c-138">valueJson</span></span>|<span data-ttu-id="4457c-139">String</span><span class="sxs-lookup"><span data-stu-id="4457c-139">String</span></span>|<span data-ttu-id="4457c-140">Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4457c-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4457c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4457c-141">Response</span></span>
<span data-ttu-id="4457c-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4457c-142">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4457c-143">Пример</span><span class="sxs-lookup"><span data-stu-id="4457c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4457c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4457c-144">Request</span></span>
<span data-ttu-id="4457c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4457c-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="4457c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4457c-146">Response</span></span>
<span data-ttu-id="4457c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4457c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```







