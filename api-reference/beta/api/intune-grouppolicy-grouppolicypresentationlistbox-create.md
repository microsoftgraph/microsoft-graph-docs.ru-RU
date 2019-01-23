---
title: Создание groupPolicyPresentationListBox
description: Создание нового объекта groupPolicyPresentationListBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d080fe046af88939d4c505f3848d1a7f2b1f67d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430667"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="a35bd-103">Создание groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="a35bd-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="a35bd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a35bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a35bd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a35bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a35bd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a35bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a35bd-107">Создание нового объекта [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="a35bd-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a35bd-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a35bd-108">Prerequisites</span></span>
<span data-ttu-id="a35bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a35bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a35bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a35bd-111">Permission type</span></span>|<span data-ttu-id="a35bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a35bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a35bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a35bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a35bd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a35bd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a35bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a35bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a35bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a35bd-116">Not supported.</span></span>|
|<span data-ttu-id="a35bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a35bd-117">Application</span></span>|<span data-ttu-id="a35bd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a35bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a35bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a35bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="a35bd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a35bd-120">Request headers</span></span>
|<span data-ttu-id="a35bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a35bd-121">Header</span></span>|<span data-ttu-id="a35bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a35bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a35bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a35bd-123">Authorization</span></span>|<span data-ttu-id="a35bd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a35bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a35bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a35bd-125">Accept</span></span>|<span data-ttu-id="a35bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a35bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a35bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a35bd-127">Request body</span></span>
<span data-ttu-id="a35bd-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="a35bd-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="a35bd-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationListBox.</span><span class="sxs-lookup"><span data-stu-id="a35bd-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="a35bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a35bd-130">Property</span></span>|<span data-ttu-id="a35bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a35bd-131">Type</span></span>|<span data-ttu-id="a35bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a35bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35bd-133">label</span><span class="sxs-lookup"><span data-stu-id="a35bd-133">label</span></span>|<span data-ttu-id="a35bd-134">String</span><span class="sxs-lookup"><span data-stu-id="a35bd-134">String</span></span>|<span data-ttu-id="a35bd-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="a35bd-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="a35bd-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="a35bd-136">The default value is empty.</span></span> <span data-ttu-id="a35bd-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a35bd-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a35bd-138">id</span><span class="sxs-lookup"><span data-stu-id="a35bd-138">id</span></span>|<span data-ttu-id="a35bd-139">String</span><span class="sxs-lookup"><span data-stu-id="a35bd-139">String</span></span>|<span data-ttu-id="a35bd-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a35bd-140">Key of the entity.</span></span> <span data-ttu-id="a35bd-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a35bd-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a35bd-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a35bd-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a35bd-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a35bd-143">DateTimeOffset</span></span>|<span data-ttu-id="a35bd-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a35bd-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="a35bd-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="a35bd-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="a35bd-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="a35bd-146">explicitValue</span></span>|<span data-ttu-id="a35bd-147">Логический</span><span class="sxs-lookup"><span data-stu-id="a35bd-147">Boolean</span></span>|<span data-ttu-id="a35bd-148">Если этот параметр указан true пользователя необходимо указать значение подраздела реестра и имя подраздела реестра.</span><span class="sxs-lookup"><span data-stu-id="a35bd-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="a35bd-149">В списке существует два столбца: в поле имя и для данных.</span><span class="sxs-lookup"><span data-stu-id="a35bd-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="a35bd-150">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="a35bd-150">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="a35bd-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a35bd-151">Response</span></span>
<span data-ttu-id="a35bd-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a35bd-152">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a35bd-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a35bd-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a35bd-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a35bd-154">Request</span></span>
<span data-ttu-id="a35bd-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a35bd-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="a35bd-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a35bd-156">Response</span></span>
<span data-ttu-id="a35bd-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a35bd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




