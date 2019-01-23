---
title: Обновление groupPolicyPresentationListBox
description: Обновление свойства объекта groupPolicyPresentationListBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b443dadcfd913dfd22b2961dea34087ed64a289
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430864"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="c7d09-103">Обновление groupPolicyPresentationListBox</span><span class="sxs-lookup"><span data-stu-id="c7d09-103">Update groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="c7d09-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7d09-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7d09-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7d09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7d09-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7d09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d09-107">Обновление свойства объекта [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="c7d09-107">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7d09-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c7d09-108">Prerequisites</span></span>
<span data-ttu-id="c7d09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7d09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7d09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7d09-111">Permission type</span></span>|<span data-ttu-id="c7d09-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7d09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7d09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7d09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d09-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d09-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c7d09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7d09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7d09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7d09-116">Not supported.</span></span>|
|<span data-ttu-id="c7d09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7d09-117">Application</span></span>|<span data-ttu-id="c7d09-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7d09-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7d09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7d09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="c7d09-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7d09-120">Request headers</span></span>
|<span data-ttu-id="c7d09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7d09-121">Header</span></span>|<span data-ttu-id="c7d09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7d09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7d09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7d09-123">Authorization</span></span>|<span data-ttu-id="c7d09-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7d09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7d09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7d09-125">Accept</span></span>|<span data-ttu-id="c7d09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7d09-127">Request body</span></span>
<span data-ttu-id="c7d09-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .</span><span class="sxs-lookup"><span data-stu-id="c7d09-128">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="c7d09-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span><span class="sxs-lookup"><span data-stu-id="c7d09-129">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="c7d09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7d09-130">Property</span></span>|<span data-ttu-id="c7d09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7d09-131">Type</span></span>|<span data-ttu-id="c7d09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7d09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7d09-133">label</span><span class="sxs-lookup"><span data-stu-id="c7d09-133">label</span></span>|<span data-ttu-id="c7d09-134">String</span><span class="sxs-lookup"><span data-stu-id="c7d09-134">String</span></span>|<span data-ttu-id="c7d09-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="c7d09-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c7d09-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="c7d09-136">The default value is empty.</span></span> <span data-ttu-id="c7d09-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c7d09-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c7d09-138">id</span><span class="sxs-lookup"><span data-stu-id="c7d09-138">id</span></span>|<span data-ttu-id="c7d09-139">String</span><span class="sxs-lookup"><span data-stu-id="c7d09-139">String</span></span>|<span data-ttu-id="c7d09-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7d09-140">Key of the entity.</span></span> <span data-ttu-id="c7d09-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c7d09-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c7d09-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d09-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c7d09-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d09-143">DateTimeOffset</span></span>|<span data-ttu-id="c7d09-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7d09-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c7d09-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c7d09-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c7d09-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="c7d09-146">explicitValue</span></span>|<span data-ttu-id="c7d09-147">Логический</span><span class="sxs-lookup"><span data-stu-id="c7d09-147">Boolean</span></span>|<span data-ttu-id="c7d09-148">Если этот параметр указан true пользователя необходимо указать значение подраздела реестра и имя подраздела реестра.</span><span class="sxs-lookup"><span data-stu-id="c7d09-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="c7d09-149">В списке существует два столбца: в поле имя и для данных.</span><span class="sxs-lookup"><span data-stu-id="c7d09-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="c7d09-150">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="c7d09-150">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="c7d09-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7d09-151">Response</span></span>
<span data-ttu-id="c7d09-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7d09-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d09-153">Пример</span><span class="sxs-lookup"><span data-stu-id="c7d09-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7d09-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7d09-154">Request</span></span>
<span data-ttu-id="c7d09-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7d09-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="c7d09-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7d09-156">Response</span></span>
<span data-ttu-id="c7d09-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7d09-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




