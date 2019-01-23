---
title: Обновление groupPolicyPresentationValueLongDecimal
description: Обновление свойства объекта groupPolicyPresentationValueLongDecimal.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3aa3ad13f449bb8671688b94c5fb2530207fd2bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430762"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="28738-103">Обновление groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="28738-103">Update groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="28738-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="28738-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28738-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28738-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28738-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28738-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28738-107">Обновление свойства объекта [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="28738-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28738-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="28738-108">Prerequisites</span></span>
<span data-ttu-id="28738-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="28738-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28738-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28738-111">Permission type</span></span>|<span data-ttu-id="28738-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28738-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28738-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28738-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28738-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28738-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28738-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28738-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28738-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28738-116">Not supported.</span></span>|
|<span data-ttu-id="28738-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28738-117">Application</span></span>|<span data-ttu-id="28738-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28738-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28738-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28738-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="28738-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28738-120">Request headers</span></span>
|<span data-ttu-id="28738-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28738-121">Header</span></span>|<span data-ttu-id="28738-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28738-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28738-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28738-123">Authorization</span></span>|<span data-ttu-id="28738-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="28738-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28738-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28738-125">Accept</span></span>|<span data-ttu-id="28738-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28738-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28738-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28738-127">Request body</span></span>
<span data-ttu-id="28738-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="28738-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="28738-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="28738-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="28738-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28738-130">Property</span></span>|<span data-ttu-id="28738-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28738-131">Type</span></span>|<span data-ttu-id="28738-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28738-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28738-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28738-133">lastModifiedDateTime</span></span>|<span data-ttu-id="28738-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28738-134">DateTimeOffset</span></span>|<span data-ttu-id="28738-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="28738-135">The date and time the object was last modified.</span></span> <span data-ttu-id="28738-136">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="28738-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="28738-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28738-137">createdDateTime</span></span>|<span data-ttu-id="28738-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28738-138">DateTimeOffset</span></span>|<span data-ttu-id="28738-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="28738-139">The date and time the object was created.</span></span> <span data-ttu-id="28738-140">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="28738-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="28738-141">id</span><span class="sxs-lookup"><span data-stu-id="28738-141">id</span></span>|<span data-ttu-id="28738-142">String</span><span class="sxs-lookup"><span data-stu-id="28738-142">String</span></span>|<span data-ttu-id="28738-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="28738-143">Key of the entity.</span></span> <span data-ttu-id="28738-144">Наследуется от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="28738-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="28738-145">value</span><span class="sxs-lookup"><span data-stu-id="28738-145">value</span></span>|<span data-ttu-id="28738-146">Int64</span><span class="sxs-lookup"><span data-stu-id="28738-146">Int64</span></span>|<span data-ttu-id="28738-147">Неподписанные длинное целое значение для связанного презентации.</span><span class="sxs-lookup"><span data-stu-id="28738-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="28738-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="28738-148">Response</span></span>
<span data-ttu-id="28738-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="28738-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28738-150">Пример</span><span class="sxs-lookup"><span data-stu-id="28738-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="28738-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="28738-151">Request</span></span>
<span data-ttu-id="28738-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28738-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="28738-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="28738-153">Response</span></span>
<span data-ttu-id="28738-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="28738-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




