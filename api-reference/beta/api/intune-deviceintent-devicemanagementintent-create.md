---
title: Создание deviceManagementIntent
description: Создание нового объекта deviceManagementIntent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 20cb05e52b7b065f2cbf1768895e9686bd4a49d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128917"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="b36c5-103">Создание deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="b36c5-103">Create deviceManagementIntent</span></span>

<span data-ttu-id="b36c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b36c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b36c5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b36c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b36c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b36c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b36c5-107">Создание нового [объекта deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)</span><span class="sxs-lookup"><span data-stu-id="b36c5-107">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b36c5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b36c5-108">Prerequisites</span></span>
<span data-ttu-id="b36c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b36c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b36c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b36c5-111">Permission type</span></span>|<span data-ttu-id="b36c5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b36c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b36c5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b36c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b36c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b36c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b36c5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b36c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b36c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b36c5-116">Not supported.</span></span>|
|<span data-ttu-id="b36c5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b36c5-117">Application</span></span>|<span data-ttu-id="b36c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b36c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b36c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b36c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="b36c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b36c5-120">Request headers</span></span>
|<span data-ttu-id="b36c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b36c5-121">Header</span></span>|<span data-ttu-id="b36c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b36c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b36c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b36c5-123">Authorization</span></span>|<span data-ttu-id="b36c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b36c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b36c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b36c5-125">Accept</span></span>|<span data-ttu-id="b36c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b36c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b36c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b36c5-127">Request body</span></span>
<span data-ttu-id="b36c5-128">В теле запроса поставляем представление JSON для объекта deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="b36c5-128">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="b36c5-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="b36c5-129">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="b36c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b36c5-130">Property</span></span>|<span data-ttu-id="b36c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b36c5-131">Type</span></span>|<span data-ttu-id="b36c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b36c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b36c5-133">id</span><span class="sxs-lookup"><span data-stu-id="b36c5-133">id</span></span>|<span data-ttu-id="b36c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b36c5-134">String</span></span>|<span data-ttu-id="b36c5-135">ID намерения</span><span class="sxs-lookup"><span data-stu-id="b36c5-135">The intent ID</span></span>|
|<span data-ttu-id="b36c5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b36c5-136">displayName</span></span>|<span data-ttu-id="b36c5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b36c5-137">String</span></span>|<span data-ttu-id="b36c5-138">Имя отображения, заданное пользователю</span><span class="sxs-lookup"><span data-stu-id="b36c5-138">The user given display name</span></span>|
|<span data-ttu-id="b36c5-139">description</span><span class="sxs-lookup"><span data-stu-id="b36c5-139">description</span></span>|<span data-ttu-id="b36c5-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b36c5-140">String</span></span>|<span data-ttu-id="b36c5-141">Описание пользователя</span><span class="sxs-lookup"><span data-stu-id="b36c5-141">The user given description</span></span>|
|<span data-ttu-id="b36c5-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b36c5-142">isAssigned</span></span>|<span data-ttu-id="b36c5-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b36c5-143">Boolean</span></span>|<span data-ttu-id="b36c5-144">Означает, назначены ли намерения пользователям</span><span class="sxs-lookup"><span data-stu-id="b36c5-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="b36c5-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b36c5-145">lastModifiedDateTime</span></span>|<span data-ttu-id="b36c5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b36c5-146">DateTimeOffset</span></span>|<span data-ttu-id="b36c5-147">Когда намерение было изменено в последний раз</span><span class="sxs-lookup"><span data-stu-id="b36c5-147">When the intent was last modified</span></span>|
|<span data-ttu-id="b36c5-148">templateId</span><span class="sxs-lookup"><span data-stu-id="b36c5-148">templateId</span></span>|<span data-ttu-id="b36c5-149">Строка</span><span class="sxs-lookup"><span data-stu-id="b36c5-149">String</span></span>|<span data-ttu-id="b36c5-150">ID шаблона, который был создан из (если таково)</span><span class="sxs-lookup"><span data-stu-id="b36c5-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="b36c5-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b36c5-151">roleScopeTagIds</span></span>|<span data-ttu-id="b36c5-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b36c5-152">String collection</span></span>|<span data-ttu-id="b36c5-153">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="b36c5-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="b36c5-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b36c5-154">Response</span></span>
<span data-ttu-id="b36c5-155">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b36c5-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b36c5-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b36c5-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="b36c5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b36c5-157">Request</span></span>
<span data-ttu-id="b36c5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b36c5-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b36c5-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b36c5-159">Response</span></span>
<span data-ttu-id="b36c5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b36c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




