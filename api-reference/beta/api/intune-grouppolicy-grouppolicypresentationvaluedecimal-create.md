---
title: Создание groupPolicyPresentationValueDecimal
description: Создание нового объекта groupPolicyPresentationValueDecimal.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32e1947ccbda3b7c7e153daf6058dfc558460a02
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431733"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="5eed8-103">Создание groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="5eed8-103">Create groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="5eed8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5eed8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5eed8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eed8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5eed8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5eed8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eed8-107">Создание нового объекта [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="5eed8-107">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5eed8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5eed8-108">Prerequisites</span></span>
<span data-ttu-id="5eed8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5eed8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5eed8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eed8-111">Permission type</span></span>|<span data-ttu-id="5eed8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eed8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eed8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eed8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5eed8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eed8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5eed8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eed8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eed8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eed8-116">Not supported.</span></span>|
|<span data-ttu-id="5eed8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eed8-117">Application</span></span>|<span data-ttu-id="5eed8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eed8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eed8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eed8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="5eed8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5eed8-120">Request headers</span></span>
|<span data-ttu-id="5eed8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5eed8-121">Header</span></span>|<span data-ttu-id="5eed8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5eed8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eed8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5eed8-123">Authorization</span></span>|<span data-ttu-id="5eed8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5eed8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eed8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5eed8-125">Accept</span></span>|<span data-ttu-id="5eed8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5eed8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eed8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5eed8-127">Request body</span></span>
<span data-ttu-id="5eed8-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="5eed8-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="5eed8-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationValueDecimal.</span><span class="sxs-lookup"><span data-stu-id="5eed8-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="5eed8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5eed8-130">Property</span></span>|<span data-ttu-id="5eed8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5eed8-131">Type</span></span>|<span data-ttu-id="5eed8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5eed8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eed8-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eed8-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5eed8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eed8-134">DateTimeOffset</span></span>|<span data-ttu-id="5eed8-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5eed8-135">The date and time the object was last modified.</span></span> <span data-ttu-id="5eed8-136">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5eed8-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5eed8-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5eed8-137">createdDateTime</span></span>|<span data-ttu-id="5eed8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eed8-138">DateTimeOffset</span></span>|<span data-ttu-id="5eed8-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5eed8-139">The date and time the object was created.</span></span> <span data-ttu-id="5eed8-140">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5eed8-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5eed8-141">id</span><span class="sxs-lookup"><span data-stu-id="5eed8-141">id</span></span>|<span data-ttu-id="5eed8-142">String</span><span class="sxs-lookup"><span data-stu-id="5eed8-142">String</span></span>|<span data-ttu-id="5eed8-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5eed8-143">Key of the entity.</span></span> <span data-ttu-id="5eed8-144">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5eed8-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="5eed8-145">value</span><span class="sxs-lookup"><span data-stu-id="5eed8-145">value</span></span>|<span data-ttu-id="5eed8-146">Int64</span><span class="sxs-lookup"><span data-stu-id="5eed8-146">Int64</span></span>|<span data-ttu-id="5eed8-147">Целое число без знака для связанного презентации.</span><span class="sxs-lookup"><span data-stu-id="5eed8-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="5eed8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eed8-148">Response</span></span>
<span data-ttu-id="5eed8-149">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5eed8-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eed8-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5eed8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5eed8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eed8-151">Request</span></span>
<span data-ttu-id="5eed8-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eed8-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="5eed8-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eed8-153">Response</span></span>
<span data-ttu-id="5eed8-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5eed8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```




