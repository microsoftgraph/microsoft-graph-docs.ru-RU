---
title: Обновление groupPolicyPresentationValueText
description: Обновление свойства объекта groupPolicyPresentationValueText.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f0a1222c9abac4cbc459f25444e3cb37d6576a7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430790"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="13c17-103">Обновление groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="13c17-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="13c17-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13c17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13c17-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13c17-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c17-107">Обновление свойства объекта [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="13c17-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c17-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="13c17-108">Prerequisites</span></span>
<span data-ttu-id="13c17-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13c17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13c17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13c17-111">Permission type</span></span>|<span data-ttu-id="13c17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13c17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13c17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13c17-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c17-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="13c17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13c17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13c17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c17-116">Not supported.</span></span>|
|<span data-ttu-id="13c17-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13c17-117">Application</span></span>|<span data-ttu-id="13c17-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13c17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13c17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="13c17-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13c17-120">Request headers</span></span>
|<span data-ttu-id="13c17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13c17-121">Header</span></span>|<span data-ttu-id="13c17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13c17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13c17-123">Authorization</span></span>|<span data-ttu-id="13c17-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="13c17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13c17-125">Accept</span></span>|<span data-ttu-id="13c17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13c17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13c17-127">Request body</span></span>
<span data-ttu-id="13c17-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="13c17-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="13c17-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span><span class="sxs-lookup"><span data-stu-id="13c17-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="13c17-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13c17-130">Property</span></span>|<span data-ttu-id="13c17-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13c17-131">Type</span></span>|<span data-ttu-id="13c17-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13c17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c17-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13c17-133">lastModifiedDateTime</span></span>|<span data-ttu-id="13c17-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c17-134">DateTimeOffset</span></span>|<span data-ttu-id="13c17-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="13c17-135">The date and time the object was last modified.</span></span> <span data-ttu-id="13c17-136">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="13c17-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="13c17-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13c17-137">createdDateTime</span></span>|<span data-ttu-id="13c17-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c17-138">DateTimeOffset</span></span>|<span data-ttu-id="13c17-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="13c17-139">The date and time the object was created.</span></span> <span data-ttu-id="13c17-140">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="13c17-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="13c17-141">id</span><span class="sxs-lookup"><span data-stu-id="13c17-141">id</span></span>|<span data-ttu-id="13c17-142">String</span><span class="sxs-lookup"><span data-stu-id="13c17-142">String</span></span>|<span data-ttu-id="13c17-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13c17-143">Key of the entity.</span></span> <span data-ttu-id="13c17-144">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="13c17-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="13c17-145">value</span><span class="sxs-lookup"><span data-stu-id="13c17-145">value</span></span>|<span data-ttu-id="13c17-146">String</span><span class="sxs-lookup"><span data-stu-id="13c17-146">String</span></span>|<span data-ttu-id="13c17-147">Строковое значение для связанного презентации.</span><span class="sxs-lookup"><span data-stu-id="13c17-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="13c17-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c17-148">Response</span></span>
<span data-ttu-id="13c17-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="13c17-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c17-150">Пример</span><span class="sxs-lookup"><span data-stu-id="13c17-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c17-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="13c17-151">Request</span></span>
<span data-ttu-id="13c17-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13c17-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="13c17-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c17-153">Response</span></span>
<span data-ttu-id="13c17-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="13c17-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




