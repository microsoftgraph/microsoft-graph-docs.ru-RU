---
title: Создание groupPolicyConfiguration
description: Создание нового объекта groupPolicyConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5ce3f8408d8a6e404ac17e865cc81bb2094c0cc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430862"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="15897-103">Создание groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="15897-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="15897-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15897-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15897-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15897-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15897-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15897-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15897-107">Создание нового объекта [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15897-107">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15897-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="15897-108">Prerequisites</span></span>
<span data-ttu-id="15897-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15897-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15897-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15897-111">Permission type</span></span>|<span data-ttu-id="15897-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15897-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15897-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15897-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15897-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15897-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15897-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15897-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15897-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15897-116">Not supported.</span></span>|
|<span data-ttu-id="15897-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15897-117">Application</span></span>|<span data-ttu-id="15897-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15897-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15897-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15897-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15897-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15897-120">Request headers</span></span>
|<span data-ttu-id="15897-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15897-121">Header</span></span>|<span data-ttu-id="15897-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15897-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15897-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15897-123">Authorization</span></span>|<span data-ttu-id="15897-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="15897-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15897-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15897-125">Accept</span></span>|<span data-ttu-id="15897-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15897-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15897-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15897-127">Request body</span></span>
<span data-ttu-id="15897-128">В тексте запроса укажите представление JSON для объекта groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="15897-128">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="15897-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyConfiguration.</span><span class="sxs-lookup"><span data-stu-id="15897-129">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="15897-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15897-130">Property</span></span>|<span data-ttu-id="15897-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15897-131">Type</span></span>|<span data-ttu-id="15897-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15897-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15897-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15897-133">createdDateTime</span></span>|<span data-ttu-id="15897-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15897-134">DateTimeOffset</span></span>|<span data-ttu-id="15897-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="15897-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="15897-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15897-136">displayName</span></span>|<span data-ttu-id="15897-137">String</span><span class="sxs-lookup"><span data-stu-id="15897-137">String</span></span>|<span data-ttu-id="15897-138">Имя объекта ресурса, предоставляемые пользователями.</span><span class="sxs-lookup"><span data-stu-id="15897-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="15897-139">description</span><span class="sxs-lookup"><span data-stu-id="15897-139">description</span></span>|<span data-ttu-id="15897-140">String</span><span class="sxs-lookup"><span data-stu-id="15897-140">String</span></span>|<span data-ttu-id="15897-141">Описание для объекта ресурса, предоставляемые пользователями.</span><span class="sxs-lookup"><span data-stu-id="15897-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="15897-142">id</span><span class="sxs-lookup"><span data-stu-id="15897-142">id</span></span>|<span data-ttu-id="15897-143">String</span><span class="sxs-lookup"><span data-stu-id="15897-143">String</span></span>|<span data-ttu-id="15897-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15897-144">Key of the entity.</span></span>|
|<span data-ttu-id="15897-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15897-145">lastModifiedDateTime</span></span>|<span data-ttu-id="15897-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15897-146">DateTimeOffset</span></span>|<span data-ttu-id="15897-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="15897-147">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="15897-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="15897-148">Response</span></span>
<span data-ttu-id="15897-149">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15897-149">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15897-150">Пример</span><span class="sxs-lookup"><span data-stu-id="15897-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="15897-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="15897-151">Request</span></span>
<span data-ttu-id="15897-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15897-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="15897-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="15897-153">Response</span></span>
<span data-ttu-id="15897-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15897-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




