---
title: Создание groupPolicyPresentationValueText
description: Создание нового объекта groupPolicyPresentationValueText.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71d21691ade34a827e06198d387c21585576297
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431681"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="e7755-103">Создание groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="e7755-103">Create groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="e7755-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7755-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7755-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7755-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7755-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7755-107">Создание нового объекта [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e7755-107">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7755-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e7755-108">Prerequisites</span></span>
<span data-ttu-id="e7755-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7755-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7755-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7755-111">Permission type</span></span>|<span data-ttu-id="e7755-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7755-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7755-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7755-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7755-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7755-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7755-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7755-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7755-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7755-116">Not supported.</span></span>|
|<span data-ttu-id="e7755-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7755-117">Application</span></span>|<span data-ttu-id="e7755-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7755-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7755-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7755-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="e7755-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7755-120">Request headers</span></span>
|<span data-ttu-id="e7755-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7755-121">Header</span></span>|<span data-ttu-id="e7755-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e7755-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7755-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7755-123">Authorization</span></span>|<span data-ttu-id="e7755-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7755-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7755-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e7755-125">Accept</span></span>|<span data-ttu-id="e7755-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7755-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7755-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7755-127">Request body</span></span>
<span data-ttu-id="e7755-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="e7755-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="e7755-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationValueText.</span><span class="sxs-lookup"><span data-stu-id="e7755-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="e7755-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7755-130">Property</span></span>|<span data-ttu-id="e7755-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7755-131">Type</span></span>|<span data-ttu-id="e7755-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7755-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7755-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7755-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e7755-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7755-134">DateTimeOffset</span></span>|<span data-ttu-id="e7755-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e7755-135">The date and time the object was last modified.</span></span> <span data-ttu-id="e7755-136">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e7755-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="e7755-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7755-137">createdDateTime</span></span>|<span data-ttu-id="e7755-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7755-138">DateTimeOffset</span></span>|<span data-ttu-id="e7755-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e7755-139">The date and time the object was created.</span></span> <span data-ttu-id="e7755-140">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e7755-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="e7755-141">id</span><span class="sxs-lookup"><span data-stu-id="e7755-141">id</span></span>|<span data-ttu-id="e7755-142">String</span><span class="sxs-lookup"><span data-stu-id="e7755-142">String</span></span>|<span data-ttu-id="e7755-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7755-143">Key of the entity.</span></span> <span data-ttu-id="e7755-144">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e7755-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="e7755-145">value</span><span class="sxs-lookup"><span data-stu-id="e7755-145">value</span></span>|<span data-ttu-id="e7755-146">String</span><span class="sxs-lookup"><span data-stu-id="e7755-146">String</span></span>|<span data-ttu-id="e7755-147">Строковое значение для связанного презентации.</span><span class="sxs-lookup"><span data-stu-id="e7755-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="e7755-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7755-148">Response</span></span>
<span data-ttu-id="e7755-149">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e7755-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7755-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e7755-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7755-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7755-151">Request</span></span>
<span data-ttu-id="e7755-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7755-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="e7755-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7755-153">Response</span></span>
<span data-ttu-id="e7755-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7755-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




