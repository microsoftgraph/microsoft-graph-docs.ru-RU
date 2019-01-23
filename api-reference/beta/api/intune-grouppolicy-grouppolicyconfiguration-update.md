---
title: Обновление groupPolicyConfiguration
description: Обновление свойства объекта groupPolicyConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30ce815eef79de3fa091daede34c758699f27bc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430858"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="d8a29-103">Обновление groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8a29-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="d8a29-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8a29-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8a29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8a29-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8a29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8a29-107">Обновление свойства объекта [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8a29-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8a29-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d8a29-108">Prerequisites</span></span>
<span data-ttu-id="d8a29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8a29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8a29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8a29-111">Permission type</span></span>|<span data-ttu-id="d8a29-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8a29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8a29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8a29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8a29-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8a29-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8a29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8a29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8a29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a29-116">Not supported.</span></span>|
|<span data-ttu-id="d8a29-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8a29-117">Application</span></span>|<span data-ttu-id="d8a29-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8a29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8a29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8a29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8a29-120">Request headers</span></span>
|<span data-ttu-id="d8a29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8a29-121">Header</span></span>|<span data-ttu-id="d8a29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8a29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8a29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8a29-123">Authorization</span></span>|<span data-ttu-id="d8a29-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d8a29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8a29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8a29-125">Accept</span></span>|<span data-ttu-id="d8a29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8a29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8a29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8a29-127">Request body</span></span>
<span data-ttu-id="d8a29-128">В тексте запроса укажите представление JSON для объекта [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8a29-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="d8a29-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8a29-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="d8a29-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8a29-130">Property</span></span>|<span data-ttu-id="d8a29-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8a29-131">Type</span></span>|<span data-ttu-id="d8a29-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8a29-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a29-133">createdDateTime</span></span>|<span data-ttu-id="d8a29-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a29-134">DateTimeOffset</span></span>|<span data-ttu-id="d8a29-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d8a29-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="d8a29-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d8a29-136">displayName</span></span>|<span data-ttu-id="d8a29-137">String</span><span class="sxs-lookup"><span data-stu-id="d8a29-137">String</span></span>|<span data-ttu-id="d8a29-138">Имя объекта ресурса, предоставляемые пользователями.</span><span class="sxs-lookup"><span data-stu-id="d8a29-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="d8a29-139">description</span><span class="sxs-lookup"><span data-stu-id="d8a29-139">description</span></span>|<span data-ttu-id="d8a29-140">String</span><span class="sxs-lookup"><span data-stu-id="d8a29-140">String</span></span>|<span data-ttu-id="d8a29-141">Описание для объекта ресурса, предоставляемые пользователями.</span><span class="sxs-lookup"><span data-stu-id="d8a29-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="d8a29-142">id</span><span class="sxs-lookup"><span data-stu-id="d8a29-142">id</span></span>|<span data-ttu-id="d8a29-143">String</span><span class="sxs-lookup"><span data-stu-id="d8a29-143">String</span></span>|<span data-ttu-id="d8a29-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8a29-144">Key of the entity.</span></span>|
|<span data-ttu-id="d8a29-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a29-145">lastModifiedDateTime</span></span>|<span data-ttu-id="d8a29-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a29-146">DateTimeOffset</span></span>|<span data-ttu-id="d8a29-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d8a29-147">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d8a29-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8a29-148">Response</span></span>
<span data-ttu-id="d8a29-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d8a29-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8a29-150">Пример</span><span class="sxs-lookup"><span data-stu-id="d8a29-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8a29-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8a29-151">Request</span></span>
<span data-ttu-id="d8a29-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8a29-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="d8a29-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8a29-153">Response</span></span>
<span data-ttu-id="d8a29-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8a29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




