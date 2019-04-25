---
title: Создание Граупполициконфигуратион
description: Создание нового объекта Граупполициконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd0c63b1d8c8df449a68cbeb64f391adb659ae64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532116"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="f92fc-103">Создание Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f92fc-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="f92fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f92fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f92fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f92fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f92fc-106">Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f92fc-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f92fc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f92fc-107">Prerequisites</span></span>
<span data-ttu-id="f92fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f92fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f92fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f92fc-110">Permission type</span></span>|<span data-ttu-id="f92fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f92fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f92fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f92fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f92fc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92fc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f92fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f92fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f92fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f92fc-115">Not supported.</span></span>|
|<span data-ttu-id="f92fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f92fc-116">Application</span></span>|<span data-ttu-id="f92fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f92fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f92fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f92fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f92fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f92fc-119">Request headers</span></span>
|<span data-ttu-id="f92fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f92fc-120">Header</span></span>|<span data-ttu-id="f92fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f92fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f92fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f92fc-122">Authorization</span></span>|<span data-ttu-id="f92fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f92fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f92fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f92fc-124">Accept</span></span>|<span data-ttu-id="f92fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f92fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f92fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f92fc-126">Request body</span></span>
<span data-ttu-id="f92fc-127">В тексте запроса добавьте представление объекта Граупполициконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f92fc-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="f92fc-128">В следующей таблице приведены свойства, необходимые при создании Граупполициконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f92fc-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="f92fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f92fc-129">Property</span></span>|<span data-ttu-id="f92fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f92fc-130">Type</span></span>|<span data-ttu-id="f92fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f92fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f92fc-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f92fc-132">createdDateTime</span></span>|<span data-ttu-id="f92fc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92fc-133">DateTimeOffset</span></span>|<span data-ttu-id="f92fc-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f92fc-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="f92fc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f92fc-135">displayName</span></span>|<span data-ttu-id="f92fc-136">String</span><span class="sxs-lookup"><span data-stu-id="f92fc-136">String</span></span>|<span data-ttu-id="f92fc-137">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="f92fc-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="f92fc-138">description</span><span class="sxs-lookup"><span data-stu-id="f92fc-138">description</span></span>|<span data-ttu-id="f92fc-139">String</span><span class="sxs-lookup"><span data-stu-id="f92fc-139">String</span></span>|<span data-ttu-id="f92fc-140">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="f92fc-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="f92fc-141">id</span><span class="sxs-lookup"><span data-stu-id="f92fc-141">id</span></span>|<span data-ttu-id="f92fc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="f92fc-142">String</span></span>|<span data-ttu-id="f92fc-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f92fc-143">Key of the entity.</span></span>|
|<span data-ttu-id="f92fc-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f92fc-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f92fc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92fc-145">DateTimeOffset</span></span>|<span data-ttu-id="f92fc-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f92fc-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="f92fc-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="f92fc-147">Response</span></span>
<span data-ttu-id="f92fc-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f92fc-148">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f92fc-149">Пример</span><span class="sxs-lookup"><span data-stu-id="f92fc-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f92fc-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f92fc-150">Request</span></span>
<span data-ttu-id="f92fc-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f92fc-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f92fc-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f92fc-152">Response</span></span>
<span data-ttu-id="f92fc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f92fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





