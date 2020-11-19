---
title: Создание Граупполиципресентатионлистбокс
description: Создание нового объекта Граупполиципресентатионлистбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3cb9d23d802537a64a9de5078bfda0f15962ec0c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49227631"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="2db2b-103">Создание Граупполиципресентатионлистбокс</span><span class="sxs-lookup"><span data-stu-id="2db2b-103">Create groupPolicyPresentationListBox</span></span>

<span data-ttu-id="2db2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2db2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2db2b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2db2b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2db2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2db2b-107">Создание нового объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="2db2b-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2db2b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2db2b-108">Prerequisites</span></span>
<span data-ttu-id="2db2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2db2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2db2b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2db2b-111">Permission type</span></span>|<span data-ttu-id="2db2b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2db2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2db2b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2db2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2db2b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2db2b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2db2b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2db2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2db2b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db2b-116">Not supported.</span></span>|
|<span data-ttu-id="2db2b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2db2b-117">Application</span></span>|<span data-ttu-id="2db2b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2db2b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2db2b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2db2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="2db2b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2db2b-120">Request headers</span></span>
|<span data-ttu-id="2db2b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2db2b-121">Header</span></span>|<span data-ttu-id="2db2b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2db2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2db2b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2db2b-123">Authorization</span></span>|<span data-ttu-id="2db2b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2db2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2db2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2db2b-125">Accept</span></span>|<span data-ttu-id="2db2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2db2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2db2b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2db2b-127">Request body</span></span>
<span data-ttu-id="2db2b-128">В тексте запроса добавьте представление объекта Граупполиципресентатионлистбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2db2b-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="2db2b-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионлистбокс.</span><span class="sxs-lookup"><span data-stu-id="2db2b-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="2db2b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2db2b-130">Property</span></span>|<span data-ttu-id="2db2b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2db2b-131">Type</span></span>|<span data-ttu-id="2db2b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2db2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2db2b-133">label</span><span class="sxs-lookup"><span data-stu-id="2db2b-133">label</span></span>|<span data-ttu-id="2db2b-134">String</span><span class="sxs-lookup"><span data-stu-id="2db2b-134">String</span></span>|<span data-ttu-id="2db2b-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="2db2b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="2db2b-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="2db2b-136">The default value is empty.</span></span> <span data-ttu-id="2db2b-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2db2b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2db2b-138">id</span><span class="sxs-lookup"><span data-stu-id="2db2b-138">id</span></span>|<span data-ttu-id="2db2b-139">String</span><span class="sxs-lookup"><span data-stu-id="2db2b-139">String</span></span>|<span data-ttu-id="2db2b-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2db2b-140">Key of the entity.</span></span> <span data-ttu-id="2db2b-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2db2b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2db2b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2db2b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="2db2b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2db2b-143">DateTimeOffset</span></span>|<span data-ttu-id="2db2b-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2db2b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="2db2b-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2db2b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2db2b-146">експлиЦитвалуе</span><span class="sxs-lookup"><span data-stu-id="2db2b-146">explicitValue</span></span>|<span data-ttu-id="2db2b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="2db2b-147">Boolean</span></span>|<span data-ttu-id="2db2b-148">Если этот параметр задан, пользователь должен указать значение подраздела реестра и имя подраздела реестра.</span><span class="sxs-lookup"><span data-stu-id="2db2b-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="2db2b-149">В списке показаны два столбца: один для имени и один для данных.</span><span class="sxs-lookup"><span data-stu-id="2db2b-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="2db2b-150">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="2db2b-150">The default value is false.</span></span>|
|<span data-ttu-id="2db2b-151">валуепрефикс</span><span class="sxs-lookup"><span data-stu-id="2db2b-151">valuePrefix</span></span>|<span data-ttu-id="2db2b-152">String</span><span class="sxs-lookup"><span data-stu-id="2db2b-152">String</span></span>|<span data-ttu-id="2db2b-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2db2b-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2db2b-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="2db2b-154">Response</span></span>
<span data-ttu-id="2db2b-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2db2b-155">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2db2b-156">Пример</span><span class="sxs-lookup"><span data-stu-id="2db2b-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="2db2b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2db2b-157">Request</span></span>
<span data-ttu-id="2db2b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2db2b-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true,
  "valuePrefix": "Value Prefix value"
}
```

### <a name="response"></a><span data-ttu-id="2db2b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2db2b-159">Response</span></span>
<span data-ttu-id="2db2b-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2db2b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




