---
title: Создание groupPolicyPresentationCheckBox
description: Создание нового объекта groupPolicyPresentationCheckBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc0d5ff04aedfbbf0e9bac3967f5f502a13e5e57
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430679"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="f9b0b-103">Создание groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="f9b0b-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="f9b0b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9b0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9b0b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9b0b-107">Создание нового объекта [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="f9b0b-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9b0b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f9b0b-108">Prerequisites</span></span>
<span data-ttu-id="f9b0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9b0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9b0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9b0b-111">Permission type</span></span>|<span data-ttu-id="f9b0b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9b0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9b0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9b0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9b0b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b0b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f9b0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9b0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9b0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-116">Not supported.</span></span>|
|<span data-ttu-id="f9b0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9b0b-117">Application</span></span>|<span data-ttu-id="f9b0b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9b0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="f9b0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9b0b-120">Request headers</span></span>
|<span data-ttu-id="f9b0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9b0b-121">Header</span></span>|<span data-ttu-id="f9b0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9b0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9b0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9b0b-123">Authorization</span></span>|<span data-ttu-id="f9b0b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f9b0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9b0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9b0b-125">Accept</span></span>|<span data-ttu-id="f9b0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9b0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9b0b-127">Request body</span></span>
<span data-ttu-id="f9b0b-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="f9b0b-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="f9b0b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9b0b-130">Property</span></span>|<span data-ttu-id="f9b0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9b0b-131">Type</span></span>|<span data-ttu-id="f9b0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9b0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9b0b-133">label</span><span class="sxs-lookup"><span data-stu-id="f9b0b-133">label</span></span>|<span data-ttu-id="f9b0b-134">String</span><span class="sxs-lookup"><span data-stu-id="f9b0b-134">String</span></span>|<span data-ttu-id="f9b0b-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f9b0b-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-136">The default value is empty.</span></span> <span data-ttu-id="f9b0b-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f9b0b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f9b0b-138">id</span><span class="sxs-lookup"><span data-stu-id="f9b0b-138">id</span></span>|<span data-ttu-id="f9b0b-139">String</span><span class="sxs-lookup"><span data-stu-id="f9b0b-139">String</span></span>|<span data-ttu-id="f9b0b-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-140">Key of the entity.</span></span> <span data-ttu-id="f9b0b-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f9b0b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f9b0b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9b0b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f9b0b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9b0b-143">DateTimeOffset</span></span>|<span data-ttu-id="f9b0b-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="f9b0b-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="f9b0b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f9b0b-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="f9b0b-146">defaultChecked</span></span>|<span data-ttu-id="f9b0b-147">Логический</span><span class="sxs-lookup"><span data-stu-id="f9b0b-147">Boolean</span></span>|<span data-ttu-id="f9b0b-148">Значение по умолчанию для флажка.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-148">Default value for the check box.</span></span> <span data-ttu-id="f9b0b-149">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="f9b0b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9b0b-150">Response</span></span>
<span data-ttu-id="f9b0b-151">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b0b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="f9b0b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9b0b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9b0b-153">Request</span></span>
<span data-ttu-id="f9b0b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="f9b0b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9b0b-155">Response</span></span>
<span data-ttu-id="f9b0b-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f9b0b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




