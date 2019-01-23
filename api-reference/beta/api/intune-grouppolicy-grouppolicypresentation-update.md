---
title: Обновление groupPolicyPresentation
description: Обновление свойства объекта groupPolicyPresentation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 26f185d1474402f77f8dab09c500a1c11892f77b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431702"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="4feeb-103">Обновление groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="4feeb-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="4feeb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4feeb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4feeb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4feeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4feeb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4feeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4feeb-107">Обновление свойства объекта [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="4feeb-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4feeb-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4feeb-108">Prerequisites</span></span>
<span data-ttu-id="4feeb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4feeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4feeb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4feeb-111">Permission type</span></span>|<span data-ttu-id="4feeb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4feeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4feeb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4feeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4feeb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4feeb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4feeb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4feeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4feeb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4feeb-116">Not supported.</span></span>|
|<span data-ttu-id="4feeb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4feeb-117">Application</span></span>|<span data-ttu-id="4feeb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4feeb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4feeb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4feeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="4feeb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4feeb-120">Request headers</span></span>
|<span data-ttu-id="4feeb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4feeb-121">Header</span></span>|<span data-ttu-id="4feeb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4feeb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4feeb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4feeb-123">Authorization</span></span>|<span data-ttu-id="4feeb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4feeb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4feeb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4feeb-125">Accept</span></span>|<span data-ttu-id="4feeb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4feeb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4feeb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4feeb-127">Request body</span></span>
<span data-ttu-id="4feeb-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="4feeb-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="4feeb-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span><span class="sxs-lookup"><span data-stu-id="4feeb-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="4feeb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4feeb-130">Property</span></span>|<span data-ttu-id="4feeb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4feeb-131">Type</span></span>|<span data-ttu-id="4feeb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4feeb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4feeb-133">label</span><span class="sxs-lookup"><span data-stu-id="4feeb-133">label</span></span>|<span data-ttu-id="4feeb-134">String</span><span class="sxs-lookup"><span data-stu-id="4feeb-134">String</span></span>|<span data-ttu-id="4feeb-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="4feeb-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="4feeb-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="4feeb-136">The default value is empty.</span></span>|
|<span data-ttu-id="4feeb-137">id</span><span class="sxs-lookup"><span data-stu-id="4feeb-137">id</span></span>|<span data-ttu-id="4feeb-138">String</span><span class="sxs-lookup"><span data-stu-id="4feeb-138">String</span></span>|<span data-ttu-id="4feeb-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4feeb-139">Key of the entity.</span></span>|
|<span data-ttu-id="4feeb-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4feeb-140">lastModifiedDateTime</span></span>|<span data-ttu-id="4feeb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4feeb-141">DateTimeOffset</span></span>|<span data-ttu-id="4feeb-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4feeb-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="4feeb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4feeb-143">Response</span></span>
<span data-ttu-id="4feeb-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4feeb-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4feeb-145">Пример</span><span class="sxs-lookup"><span data-stu-id="4feeb-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="4feeb-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4feeb-146">Request</span></span>
<span data-ttu-id="4feeb-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4feeb-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="4feeb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4feeb-148">Response</span></span>
<span data-ttu-id="4feeb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4feeb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




