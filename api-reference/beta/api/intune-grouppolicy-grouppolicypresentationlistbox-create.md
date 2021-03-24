---
title: Создание groupPolicyPresentationListBox
description: Создайте новый объект GroupPolicyPresentationListBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 561a591e61ef5d6872f2eec63c24964b7827ce43
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135392"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="9e873-103">Создание groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="9e873-103">Create groupPolicyPresentationListBox</span></span>

<span data-ttu-id="9e873-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e873-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e873-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e873-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e873-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e873-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e873-107">Создайте новый [объект GroupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)</span><span class="sxs-lookup"><span data-stu-id="9e873-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e873-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9e873-108">Prerequisites</span></span>
<span data-ttu-id="9e873-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e873-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e873-111">Permission type</span></span>|<span data-ttu-id="9e873-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e873-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e873-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e873-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e873-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e873-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e873-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e873-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e873-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e873-116">Not supported.</span></span>|
|<span data-ttu-id="9e873-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e873-117">Application</span></span>|<span data-ttu-id="9e873-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e873-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e873-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e873-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="9e873-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9e873-120">Request headers</span></span>
|<span data-ttu-id="9e873-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e873-121">Header</span></span>|<span data-ttu-id="9e873-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9e873-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e873-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e873-123">Authorization</span></span>|<span data-ttu-id="9e873-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e873-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e873-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e873-125">Accept</span></span>|<span data-ttu-id="9e873-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e873-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e873-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e873-127">Request body</span></span>
<span data-ttu-id="9e873-128">В теле запроса поставляем представление JSON для объекта groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="9e873-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="9e873-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="9e873-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="9e873-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e873-130">Property</span></span>|<span data-ttu-id="9e873-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9e873-131">Type</span></span>|<span data-ttu-id="9e873-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9e873-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e873-133">label</span><span class="sxs-lookup"><span data-stu-id="9e873-133">label</span></span>|<span data-ttu-id="9e873-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9e873-134">String</span></span>|<span data-ttu-id="9e873-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="9e873-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9e873-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="9e873-136">The default value is empty.</span></span> <span data-ttu-id="9e873-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9e873-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9e873-138">id</span><span class="sxs-lookup"><span data-stu-id="9e873-138">id</span></span>|<span data-ttu-id="9e873-139">Строка</span><span class="sxs-lookup"><span data-stu-id="9e873-139">String</span></span>|<span data-ttu-id="9e873-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9e873-140">Key of the entity.</span></span> <span data-ttu-id="9e873-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9e873-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9e873-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e873-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9e873-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e873-143">DateTimeOffset</span></span>|<span data-ttu-id="9e873-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9e873-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="9e873-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9e873-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9e873-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="9e873-146">explicitValue</span></span>|<span data-ttu-id="9e873-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e873-147">Boolean</span></span>|<span data-ttu-id="9e873-148">Если этот параметр указан верно, пользователь должен указать значение подкайки реестра и имя подкайки реестра.</span><span class="sxs-lookup"><span data-stu-id="9e873-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="9e873-149">В поле списка показаны два столбца: один для имени и один для данных.</span><span class="sxs-lookup"><span data-stu-id="9e873-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="9e873-150">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="9e873-150">The default value is false.</span></span>|
|<span data-ttu-id="9e873-151">valuePrefix</span><span class="sxs-lookup"><span data-stu-id="9e873-151">valuePrefix</span></span>|<span data-ttu-id="9e873-152">String</span><span class="sxs-lookup"><span data-stu-id="9e873-152">String</span></span>|<span data-ttu-id="9e873-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9e873-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9e873-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e873-154">Response</span></span>
<span data-ttu-id="9e873-155">В случае успеха этот метод возвращает код отклика и `201 Created` [объект GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9e873-155">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e873-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9e873-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e873-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e873-157">Request</span></span>
<span data-ttu-id="9e873-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e873-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e873-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e873-159">Response</span></span>
<span data-ttu-id="9e873-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e873-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




