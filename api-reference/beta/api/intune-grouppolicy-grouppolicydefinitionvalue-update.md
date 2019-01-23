---
title: Обновление groupPolicyDefinitionValue
description: Обновление свойства объекта groupPolicyDefinitionValue.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d346a40e5ee8c2cba6f1510cf52d747e85a0b788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430584"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="e8885-103">Обновление groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e8885-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="e8885-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8885-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8885-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8885-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8885-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8885-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8885-107">Обновление свойства объекта [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="e8885-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8885-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e8885-108">Prerequisites</span></span>
<span data-ttu-id="e8885-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8885-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e8885-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8885-111">Permission type</span></span>|<span data-ttu-id="e8885-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8885-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8885-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8885-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8885-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8885-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8885-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8885-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8885-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8885-116">Not supported.</span></span>|
|<span data-ttu-id="e8885-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8885-117">Application</span></span>|<span data-ttu-id="e8885-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8885-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8885-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8885-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="e8885-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8885-120">Request headers</span></span>
|<span data-ttu-id="e8885-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8885-121">Header</span></span>|<span data-ttu-id="e8885-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8885-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8885-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8885-123">Authorization</span></span>|<span data-ttu-id="e8885-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e8885-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8885-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8885-125">Accept</span></span>|<span data-ttu-id="e8885-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8885-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8885-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8885-127">Request body</span></span>
<span data-ttu-id="e8885-128">В тексте запроса укажите представление JSON для объекта [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="e8885-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="e8885-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="e8885-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="e8885-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8885-130">Property</span></span>|<span data-ttu-id="e8885-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8885-131">Type</span></span>|<span data-ttu-id="e8885-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8885-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8885-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8885-133">createdDateTime</span></span>|<span data-ttu-id="e8885-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8885-134">DateTimeOffset</span></span>|<span data-ttu-id="e8885-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e8885-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="e8885-136">enabled</span><span class="sxs-lookup"><span data-stu-id="e8885-136">enabled</span></span>|<span data-ttu-id="e8885-137">Логический</span><span class="sxs-lookup"><span data-stu-id="e8885-137">Boolean</span></span>|<span data-ttu-id="e8885-138">Включает или отключает определения связанного групповой политики.</span><span class="sxs-lookup"><span data-stu-id="e8885-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="e8885-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="e8885-139">configurationType</span></span>|[<span data-ttu-id="e8885-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="e8885-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="e8885-141">Указывает, как настроить значение.</span><span class="sxs-lookup"><span data-stu-id="e8885-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="e8885-142">Это может быть как политики или настройки.</span><span class="sxs-lookup"><span data-stu-id="e8885-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="e8885-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="e8885-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="e8885-144">id</span><span class="sxs-lookup"><span data-stu-id="e8885-144">id</span></span>|<span data-ttu-id="e8885-145">String</span><span class="sxs-lookup"><span data-stu-id="e8885-145">String</span></span>|<span data-ttu-id="e8885-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8885-146">Key of the entity.</span></span>|
|<span data-ttu-id="e8885-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8885-147">lastModifiedDateTime</span></span>|<span data-ttu-id="e8885-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8885-148">DateTimeOffset</span></span>|<span data-ttu-id="e8885-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e8885-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e8885-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8885-150">Response</span></span>
<span data-ttu-id="e8885-151">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8885-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8885-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e8885-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8885-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8885-153">Request</span></span>
<span data-ttu-id="e8885-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8885-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="e8885-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8885-155">Response</span></span>
<span data-ttu-id="e8885-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8885-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




