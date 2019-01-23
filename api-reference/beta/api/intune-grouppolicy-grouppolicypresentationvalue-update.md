---
title: Обновление groupPolicyPresentationValue
description: Обновление свойства объекта groupPolicyPresentationValue.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfec8c5c0a228bf4ba1ed360339d4194cc877faf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430768"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="3531f-103">Обновление groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="3531f-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="3531f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3531f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3531f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3531f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3531f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3531f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3531f-107">Обновление свойства объекта [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="3531f-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3531f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3531f-108">Prerequisites</span></span>
<span data-ttu-id="3531f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3531f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3531f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3531f-111">Permission type</span></span>|<span data-ttu-id="3531f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3531f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3531f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3531f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3531f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3531f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3531f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3531f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3531f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3531f-116">Not supported.</span></span>|
|<span data-ttu-id="3531f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3531f-117">Application</span></span>|<span data-ttu-id="3531f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3531f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3531f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3531f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="3531f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3531f-120">Request headers</span></span>
|<span data-ttu-id="3531f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3531f-121">Header</span></span>|<span data-ttu-id="3531f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3531f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3531f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3531f-123">Authorization</span></span>|<span data-ttu-id="3531f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3531f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3531f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3531f-125">Accept</span></span>|<span data-ttu-id="3531f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3531f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3531f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3531f-127">Request body</span></span>
<span data-ttu-id="3531f-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="3531f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="3531f-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="3531f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="3531f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3531f-130">Property</span></span>|<span data-ttu-id="3531f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3531f-131">Type</span></span>|<span data-ttu-id="3531f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3531f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3531f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3531f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3531f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3531f-134">DateTimeOffset</span></span>|<span data-ttu-id="3531f-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3531f-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="3531f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3531f-136">createdDateTime</span></span>|<span data-ttu-id="3531f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3531f-137">DateTimeOffset</span></span>|<span data-ttu-id="3531f-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3531f-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="3531f-139">id</span><span class="sxs-lookup"><span data-stu-id="3531f-139">id</span></span>|<span data-ttu-id="3531f-140">String</span><span class="sxs-lookup"><span data-stu-id="3531f-140">String</span></span>|<span data-ttu-id="3531f-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3531f-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3531f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3531f-142">Response</span></span>
<span data-ttu-id="3531f-143">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3531f-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3531f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3531f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3531f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3531f-145">Request</span></span>
<span data-ttu-id="3531f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3531f-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="3531f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3531f-147">Response</span></span>
<span data-ttu-id="3531f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3531f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




