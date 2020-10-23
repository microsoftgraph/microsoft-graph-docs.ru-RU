---
title: Создание Девицеманажементкомплекссеттингинстанце
description: Создание нового объекта Девицеманажементкомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97edf735025a02e10318404dbdcdd4356ed73bb9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726166"
---
# <a name="create-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="e588b-103">Создание Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="e588b-103">Create deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="e588b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e588b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e588b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e588b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e588b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e588b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e588b-107">Создание нового объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="e588b-107">Create a new [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e588b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e588b-108">Prerequisites</span></span>
<span data-ttu-id="e588b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e588b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e588b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e588b-111">Permission type</span></span>|<span data-ttu-id="e588b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e588b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e588b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e588b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e588b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e588b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e588b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e588b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e588b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e588b-116">Not supported.</span></span>|
|<span data-ttu-id="e588b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e588b-117">Application</span></span>|<span data-ttu-id="e588b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e588b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e588b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e588b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e588b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e588b-120">Request headers</span></span>
|<span data-ttu-id="e588b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e588b-121">Header</span></span>|<span data-ttu-id="e588b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e588b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e588b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e588b-123">Authorization</span></span>|<span data-ttu-id="e588b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e588b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e588b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e588b-125">Accept</span></span>|<span data-ttu-id="e588b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e588b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e588b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e588b-127">Request body</span></span>
<span data-ttu-id="e588b-128">В тексте запроса добавьте представление объекта Девицеманажементкомплекссеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e588b-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingInstance object.</span></span>

<span data-ttu-id="e588b-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементкомплекссеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="e588b-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingInstance.</span></span>

|<span data-ttu-id="e588b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e588b-130">Property</span></span>|<span data-ttu-id="e588b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e588b-131">Type</span></span>|<span data-ttu-id="e588b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e588b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e588b-133">id</span><span class="sxs-lookup"><span data-stu-id="e588b-133">id</span></span>|<span data-ttu-id="e588b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e588b-134">String</span></span>|<span data-ttu-id="e588b-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e588b-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="e588b-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="e588b-136">definitionId</span></span>|<span data-ttu-id="e588b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e588b-137">String</span></span>|<span data-ttu-id="e588b-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e588b-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="e588b-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="e588b-139">valueJson</span></span>|<span data-ttu-id="e588b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e588b-140">String</span></span>|<span data-ttu-id="e588b-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e588b-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e588b-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e588b-142">Response</span></span>
<span data-ttu-id="e588b-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e588b-143">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e588b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e588b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e588b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e588b-145">Request</span></span>
<span data-ttu-id="e588b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e588b-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e588b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e588b-147">Response</span></span>
<span data-ttu-id="e588b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e588b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





