---
title: Обновление groupPolicyPresentationCheckBox
description: Обновление свойства объекта groupPolicyPresentationCheckBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4150e662109b9dc9d0ebee6a66be12ad1c2473bc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430767"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="c0583-103">Обновление groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="c0583-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="c0583-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0583-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0583-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0583-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0583-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0583-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0583-107">Обновление свойства объекта [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="c0583-107">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0583-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c0583-108">Prerequisites</span></span>
<span data-ttu-id="c0583-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0583-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0583-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0583-111">Permission type</span></span>|<span data-ttu-id="c0583-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0583-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0583-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0583-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0583-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0583-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0583-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0583-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0583-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0583-116">Not supported.</span></span>|
|<span data-ttu-id="c0583-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0583-117">Application</span></span>|<span data-ttu-id="c0583-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0583-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0583-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0583-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0583-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0583-120">Request headers</span></span>
|<span data-ttu-id="c0583-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0583-121">Header</span></span>|<span data-ttu-id="c0583-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0583-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0583-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0583-123">Authorization</span></span>|<span data-ttu-id="c0583-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c0583-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0583-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0583-125">Accept</span></span>|<span data-ttu-id="c0583-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0583-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0583-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0583-127">Request body</span></span>
<span data-ttu-id="c0583-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="c0583-128">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="c0583-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span><span class="sxs-lookup"><span data-stu-id="c0583-129">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="c0583-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0583-130">Property</span></span>|<span data-ttu-id="c0583-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c0583-131">Type</span></span>|<span data-ttu-id="c0583-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c0583-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0583-133">label</span><span class="sxs-lookup"><span data-stu-id="c0583-133">label</span></span>|<span data-ttu-id="c0583-134">String</span><span class="sxs-lookup"><span data-stu-id="c0583-134">String</span></span>|<span data-ttu-id="c0583-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="c0583-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c0583-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="c0583-136">The default value is empty.</span></span> <span data-ttu-id="c0583-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c0583-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c0583-138">id</span><span class="sxs-lookup"><span data-stu-id="c0583-138">id</span></span>|<span data-ttu-id="c0583-139">String</span><span class="sxs-lookup"><span data-stu-id="c0583-139">String</span></span>|<span data-ttu-id="c0583-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c0583-140">Key of the entity.</span></span> <span data-ttu-id="c0583-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c0583-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c0583-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0583-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c0583-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0583-143">DateTimeOffset</span></span>|<span data-ttu-id="c0583-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c0583-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c0583-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c0583-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c0583-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="c0583-146">defaultChecked</span></span>|<span data-ttu-id="c0583-147">Логический</span><span class="sxs-lookup"><span data-stu-id="c0583-147">Boolean</span></span>|<span data-ttu-id="c0583-148">Значение по умолчанию для флажка.</span><span class="sxs-lookup"><span data-stu-id="c0583-148">Default value for the check box.</span></span> <span data-ttu-id="c0583-149">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="c0583-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="c0583-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0583-150">Response</span></span>
<span data-ttu-id="c0583-151">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c0583-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0583-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c0583-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0583-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0583-153">Request</span></span>
<span data-ttu-id="c0583-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0583-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="c0583-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0583-155">Response</span></span>
<span data-ttu-id="c0583-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c0583-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```




