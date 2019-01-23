---
title: Создание groupPolicyPresentationValueLongDecimal
description: Создание нового объекта groupPolicyPresentationValueLongDecimal.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 51dacbea1970d042d4fe1fb5b3b2bd42f522b131
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430797"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="7bdec-103">Создание groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="7bdec-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="7bdec-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7bdec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7bdec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bdec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bdec-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bdec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bdec-107">Создание нового объекта [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="7bdec-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bdec-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7bdec-108">Prerequisites</span></span>
<span data-ttu-id="7bdec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bdec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7bdec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bdec-111">Permission type</span></span>|<span data-ttu-id="7bdec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bdec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bdec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bdec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bdec-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bdec-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7bdec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bdec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bdec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bdec-116">Not supported.</span></span>|
|<span data-ttu-id="7bdec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bdec-117">Application</span></span>|<span data-ttu-id="7bdec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bdec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bdec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bdec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="7bdec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bdec-120">Request headers</span></span>
|<span data-ttu-id="7bdec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bdec-121">Header</span></span>|<span data-ttu-id="7bdec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7bdec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bdec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bdec-123">Authorization</span></span>|<span data-ttu-id="7bdec-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7bdec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bdec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7bdec-125">Accept</span></span>|<span data-ttu-id="7bdec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bdec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bdec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bdec-127">Request body</span></span>
<span data-ttu-id="7bdec-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="7bdec-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="7bdec-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationValueLongDecimal.</span><span class="sxs-lookup"><span data-stu-id="7bdec-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="7bdec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bdec-130">Property</span></span>|<span data-ttu-id="7bdec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7bdec-131">Type</span></span>|<span data-ttu-id="7bdec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7bdec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bdec-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bdec-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7bdec-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bdec-134">DateTimeOffset</span></span>|<span data-ttu-id="7bdec-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7bdec-135">The date and time the object was last modified.</span></span> <span data-ttu-id="7bdec-136">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7bdec-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7bdec-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bdec-137">createdDateTime</span></span>|<span data-ttu-id="7bdec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bdec-138">DateTimeOffset</span></span>|<span data-ttu-id="7bdec-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7bdec-139">The date and time the object was created.</span></span> <span data-ttu-id="7bdec-140">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7bdec-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7bdec-141">id</span><span class="sxs-lookup"><span data-stu-id="7bdec-141">id</span></span>|<span data-ttu-id="7bdec-142">String</span><span class="sxs-lookup"><span data-stu-id="7bdec-142">String</span></span>|<span data-ttu-id="7bdec-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7bdec-143">Key of the entity.</span></span> <span data-ttu-id="7bdec-144">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7bdec-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7bdec-145">value</span><span class="sxs-lookup"><span data-stu-id="7bdec-145">value</span></span>|<span data-ttu-id="7bdec-146">Int64</span><span class="sxs-lookup"><span data-stu-id="7bdec-146">Int64</span></span>|<span data-ttu-id="7bdec-147">Неподписанные длинное целое значение для связанного презентации.</span><span class="sxs-lookup"><span data-stu-id="7bdec-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="7bdec-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bdec-148">Response</span></span>
<span data-ttu-id="7bdec-149">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7bdec-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bdec-150">Пример</span><span class="sxs-lookup"><span data-stu-id="7bdec-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bdec-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bdec-151">Request</span></span>
<span data-ttu-id="7bdec-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bdec-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="7bdec-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bdec-153">Response</span></span>
<span data-ttu-id="7bdec-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7bdec-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




