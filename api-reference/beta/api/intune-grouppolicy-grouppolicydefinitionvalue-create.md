---
title: Создание groupPolicyDefinitionValue
description: Создание нового объекта groupPolicyDefinitionValue.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d859a1405c9b2879da1c9b57f31c1ffde3ce0cfc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430681"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="49f65-103">Создание groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="49f65-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="49f65-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49f65-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49f65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49f65-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49f65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49f65-107">Создание нового объекта [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="49f65-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49f65-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="49f65-108">Prerequisites</span></span>
<span data-ttu-id="49f65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="49f65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49f65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49f65-111">Permission type</span></span>|<span data-ttu-id="49f65-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49f65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49f65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49f65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49f65-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f65-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49f65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49f65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49f65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f65-116">Not supported.</span></span>|
|<span data-ttu-id="49f65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49f65-117">Application</span></span>|<span data-ttu-id="49f65-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49f65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49f65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="49f65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49f65-120">Request headers</span></span>
|<span data-ttu-id="49f65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49f65-121">Header</span></span>|<span data-ttu-id="49f65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49f65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49f65-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49f65-123">Authorization</span></span>|<span data-ttu-id="49f65-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="49f65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49f65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49f65-125">Accept</span></span>|<span data-ttu-id="49f65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49f65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f65-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49f65-127">Request body</span></span>
<span data-ttu-id="49f65-128">В тексте запроса укажите представление JSON для объекта groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="49f65-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="49f65-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="49f65-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="49f65-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49f65-130">Property</span></span>|<span data-ttu-id="49f65-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49f65-131">Type</span></span>|<span data-ttu-id="49f65-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49f65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f65-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49f65-133">createdDateTime</span></span>|<span data-ttu-id="49f65-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f65-134">DateTimeOffset</span></span>|<span data-ttu-id="49f65-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="49f65-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="49f65-136">enabled</span><span class="sxs-lookup"><span data-stu-id="49f65-136">enabled</span></span>|<span data-ttu-id="49f65-137">Логический</span><span class="sxs-lookup"><span data-stu-id="49f65-137">Boolean</span></span>|<span data-ttu-id="49f65-138">Включает или отключает определения связанного групповой политики.</span><span class="sxs-lookup"><span data-stu-id="49f65-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="49f65-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="49f65-139">configurationType</span></span>|[<span data-ttu-id="49f65-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="49f65-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="49f65-141">Указывает, как настроить значение.</span><span class="sxs-lookup"><span data-stu-id="49f65-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="49f65-142">Это может быть как политики или настройки.</span><span class="sxs-lookup"><span data-stu-id="49f65-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="49f65-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="49f65-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="49f65-144">id</span><span class="sxs-lookup"><span data-stu-id="49f65-144">id</span></span>|<span data-ttu-id="49f65-145">String</span><span class="sxs-lookup"><span data-stu-id="49f65-145">String</span></span>|<span data-ttu-id="49f65-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49f65-146">Key of the entity.</span></span>|
|<span data-ttu-id="49f65-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49f65-147">lastModifiedDateTime</span></span>|<span data-ttu-id="49f65-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f65-148">DateTimeOffset</span></span>|<span data-ttu-id="49f65-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="49f65-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="49f65-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f65-150">Response</span></span>
<span data-ttu-id="49f65-151">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="49f65-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f65-152">Пример</span><span class="sxs-lookup"><span data-stu-id="49f65-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="49f65-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="49f65-153">Request</span></span>
<span data-ttu-id="49f65-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49f65-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="49f65-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f65-155">Response</span></span>
<span data-ttu-id="49f65-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="49f65-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




