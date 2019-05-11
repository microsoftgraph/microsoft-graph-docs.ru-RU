---
title: Создание Девицеманажементколлектионсеттингинстанце
description: Создание нового объекта Девицеманажементколлектионсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8d1afab724be719e1b8886f395596ba721706f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916759"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="73bac-103">Создание Девицеманажементколлектионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="73bac-103">Create deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="73bac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73bac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73bac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73bac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73bac-106">Создание нового объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="73bac-106">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73bac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73bac-107">Prerequisites</span></span>
<span data-ttu-id="73bac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73bac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73bac-110">Permission type</span></span>|<span data-ttu-id="73bac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73bac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73bac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73bac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73bac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73bac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73bac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73bac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73bac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73bac-115">Not supported.</span></span>|
|<span data-ttu-id="73bac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73bac-116">Application</span></span>|<span data-ttu-id="73bac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73bac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73bac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73bac-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="73bac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73bac-119">Request headers</span></span>
|<span data-ttu-id="73bac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73bac-120">Header</span></span>|<span data-ttu-id="73bac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="73bac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73bac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73bac-122">Authorization</span></span>|<span data-ttu-id="73bac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73bac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73bac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="73bac-124">Accept</span></span>|<span data-ttu-id="73bac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73bac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73bac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73bac-126">Request body</span></span>
<span data-ttu-id="73bac-127">В тексте запроса добавьте представление объекта Девицеманажементколлектионсеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73bac-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="73bac-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементколлектионсеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="73bac-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="73bac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="73bac-129">Property</span></span>|<span data-ttu-id="73bac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="73bac-130">Type</span></span>|<span data-ttu-id="73bac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="73bac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73bac-132">id</span><span class="sxs-lookup"><span data-stu-id="73bac-132">id</span></span>|<span data-ttu-id="73bac-133">Строка</span><span class="sxs-lookup"><span data-stu-id="73bac-133">String</span></span>|<span data-ttu-id="73bac-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="73bac-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="73bac-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="73bac-135">definitionId</span></span>|<span data-ttu-id="73bac-136">Строка</span><span class="sxs-lookup"><span data-stu-id="73bac-136">String</span></span>|<span data-ttu-id="73bac-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="73bac-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="73bac-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="73bac-138">valueJson</span></span>|<span data-ttu-id="73bac-139">Строка</span><span class="sxs-lookup"><span data-stu-id="73bac-139">String</span></span>|<span data-ttu-id="73bac-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="73bac-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="73bac-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="73bac-141">Response</span></span>
<span data-ttu-id="73bac-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73bac-142">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73bac-143">Пример</span><span class="sxs-lookup"><span data-stu-id="73bac-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="73bac-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="73bac-144">Request</span></span>
<span data-ttu-id="73bac-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73bac-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="73bac-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="73bac-146">Response</span></span>
<span data-ttu-id="73bac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73bac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




