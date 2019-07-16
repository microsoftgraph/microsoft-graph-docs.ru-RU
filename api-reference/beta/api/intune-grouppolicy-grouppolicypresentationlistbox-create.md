---
title: Создание Граупполиципресентатионлистбокс
description: Создание нового объекта Граупполиципресентатионлистбокс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebbd214e4ba46e3c02d7ca9f69730e4ec06262d6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721978"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="ddceb-103">Создание Граупполиципресентатионлистбокс</span><span class="sxs-lookup"><span data-stu-id="ddceb-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="ddceb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddceb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddceb-106">Создание нового объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="ddceb-106">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddceb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ddceb-107">Prerequisites</span></span>
<span data-ttu-id="ddceb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddceb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddceb-110">Permission type</span></span>|<span data-ttu-id="ddceb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddceb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddceb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddceb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddceb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddceb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ddceb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddceb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddceb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddceb-115">Not supported.</span></span>|
|<span data-ttu-id="ddceb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddceb-116">Application</span></span>|<span data-ttu-id="ddceb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddceb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddceb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddceb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="ddceb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddceb-119">Request headers</span></span>
|<span data-ttu-id="ddceb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddceb-120">Header</span></span>|<span data-ttu-id="ddceb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ddceb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddceb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddceb-122">Authorization</span></span>|<span data-ttu-id="ddceb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddceb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddceb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ddceb-124">Accept</span></span>|<span data-ttu-id="ddceb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddceb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddceb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ddceb-126">Request body</span></span>
<span data-ttu-id="ddceb-127">В тексте запроса добавьте представление объекта Граупполиципресентатионлистбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddceb-127">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="ddceb-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионлистбокс.</span><span class="sxs-lookup"><span data-stu-id="ddceb-128">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="ddceb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddceb-129">Property</span></span>|<span data-ttu-id="ddceb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ddceb-130">Type</span></span>|<span data-ttu-id="ddceb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ddceb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddceb-132">label</span><span class="sxs-lookup"><span data-stu-id="ddceb-132">label</span></span>|<span data-ttu-id="ddceb-133">String</span><span class="sxs-lookup"><span data-stu-id="ddceb-133">String</span></span>|<span data-ttu-id="ddceb-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="ddceb-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ddceb-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="ddceb-135">The default value is empty.</span></span> <span data-ttu-id="ddceb-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ddceb-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ddceb-137">id</span><span class="sxs-lookup"><span data-stu-id="ddceb-137">id</span></span>|<span data-ttu-id="ddceb-138">String</span><span class="sxs-lookup"><span data-stu-id="ddceb-138">String</span></span>|<span data-ttu-id="ddceb-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddceb-139">Key of the entity.</span></span> <span data-ttu-id="ddceb-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ddceb-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ddceb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddceb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ddceb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddceb-142">DateTimeOffset</span></span>|<span data-ttu-id="ddceb-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ddceb-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="ddceb-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ddceb-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ddceb-145">ЕксплиЦитвалуе</span><span class="sxs-lookup"><span data-stu-id="ddceb-145">explicitValue</span></span>|<span data-ttu-id="ddceb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddceb-146">Boolean</span></span>|<span data-ttu-id="ddceb-147">Если этот параметр задан, пользователь должен указать значение подраздела реестра и имя подраздела реестра.</span><span class="sxs-lookup"><span data-stu-id="ddceb-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="ddceb-148">В списке показаны два столбца: один для имени и один для данных.</span><span class="sxs-lookup"><span data-stu-id="ddceb-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="ddceb-149">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="ddceb-149">The default value is false.</span></span>|
|<span data-ttu-id="ddceb-150">Валуепрефикс</span><span class="sxs-lookup"><span data-stu-id="ddceb-150">valuePrefix</span></span>|<span data-ttu-id="ddceb-151">String</span><span class="sxs-lookup"><span data-stu-id="ddceb-151">String</span></span>|<span data-ttu-id="ddceb-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ddceb-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ddceb-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddceb-153">Response</span></span>
<span data-ttu-id="ddceb-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddceb-154">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddceb-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ddceb-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddceb-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddceb-156">Request</span></span>
<span data-ttu-id="ddceb-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddceb-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ddceb-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddceb-158">Response</span></span>
<span data-ttu-id="ddceb-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddceb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





