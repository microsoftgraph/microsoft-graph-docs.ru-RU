---
title: Обновление Граупполиципресентатионлистбокс
description: Обновление свойств объекта Граупполиципресентатионлистбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18b2fc5f19cd7f88948fd21f145e5a558b6a25f6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685620"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="84ee4-103">Обновление Граупполиципресентатионлистбокс</span><span class="sxs-lookup"><span data-stu-id="84ee4-103">Update groupPolicyPresentationListBox</span></span>

<span data-ttu-id="84ee4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ee4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ee4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84ee4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ee4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84ee4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ee4-107">Обновление свойств объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="84ee4-107">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84ee4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84ee4-108">Prerequisites</span></span>
<span data-ttu-id="84ee4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84ee4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84ee4-111">Permission type</span></span>|<span data-ttu-id="84ee4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84ee4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84ee4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84ee4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84ee4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ee4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84ee4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84ee4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84ee4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84ee4-116">Not supported.</span></span>|
|<span data-ttu-id="84ee4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84ee4-117">Application</span></span>|<span data-ttu-id="84ee4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ee4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84ee4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84ee4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="84ee4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84ee4-120">Request headers</span></span>
|<span data-ttu-id="84ee4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84ee4-121">Header</span></span>|<span data-ttu-id="84ee4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84ee4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84ee4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84ee4-123">Authorization</span></span>|<span data-ttu-id="84ee4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84ee4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84ee4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84ee4-125">Accept</span></span>|<span data-ttu-id="84ee4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84ee4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ee4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84ee4-127">Request body</span></span>
<span data-ttu-id="84ee4-128">В тексте запроса добавьте представление объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84ee4-128">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="84ee4-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span><span class="sxs-lookup"><span data-stu-id="84ee4-129">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="84ee4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84ee4-130">Property</span></span>|<span data-ttu-id="84ee4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84ee4-131">Type</span></span>|<span data-ttu-id="84ee4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84ee4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ee4-133">label</span><span class="sxs-lookup"><span data-stu-id="84ee4-133">label</span></span>|<span data-ttu-id="84ee4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="84ee4-134">String</span></span>|<span data-ttu-id="84ee4-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="84ee4-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="84ee4-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="84ee4-136">The default value is empty.</span></span> <span data-ttu-id="84ee4-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="84ee4-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="84ee4-138">id</span><span class="sxs-lookup"><span data-stu-id="84ee4-138">id</span></span>|<span data-ttu-id="84ee4-139">Строка</span><span class="sxs-lookup"><span data-stu-id="84ee4-139">String</span></span>|<span data-ttu-id="84ee4-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84ee4-140">Key of the entity.</span></span> <span data-ttu-id="84ee4-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="84ee4-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="84ee4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84ee4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="84ee4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84ee4-143">DateTimeOffset</span></span>|<span data-ttu-id="84ee4-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="84ee4-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="84ee4-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="84ee4-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="84ee4-146">експлиЦитвалуе</span><span class="sxs-lookup"><span data-stu-id="84ee4-146">explicitValue</span></span>|<span data-ttu-id="84ee4-147">Логический</span><span class="sxs-lookup"><span data-stu-id="84ee4-147">Boolean</span></span>|<span data-ttu-id="84ee4-148">Если этот параметр задан, пользователь должен указать значение подраздела реестра и имя подраздела реестра.</span><span class="sxs-lookup"><span data-stu-id="84ee4-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="84ee4-149">В списке показаны два столбца: один для имени и один для данных.</span><span class="sxs-lookup"><span data-stu-id="84ee4-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="84ee4-150">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="84ee4-150">The default value is false.</span></span>|
|<span data-ttu-id="84ee4-151">валуепрефикс</span><span class="sxs-lookup"><span data-stu-id="84ee4-151">valuePrefix</span></span>|<span data-ttu-id="84ee4-152">String</span><span class="sxs-lookup"><span data-stu-id="84ee4-152">String</span></span>|<span data-ttu-id="84ee4-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84ee4-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="84ee4-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="84ee4-154">Response</span></span>
<span data-ttu-id="84ee4-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84ee4-155">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84ee4-156">Пример</span><span class="sxs-lookup"><span data-stu-id="84ee4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="84ee4-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="84ee4-157">Request</span></span>
<span data-ttu-id="84ee4-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84ee4-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="84ee4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="84ee4-159">Response</span></span>
<span data-ttu-id="84ee4-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84ee4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```





