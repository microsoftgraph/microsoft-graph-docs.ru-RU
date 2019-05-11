---
title: Обновление Девицеманажементтемплате
description: Обновление свойств объекта Девицеманажементтемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c8c2ad9d9c0020157068c4e9b78bd13369365f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915869"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="38845-103">Обновление Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="38845-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="38845-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38845-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38845-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38845-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38845-106">Обновление свойств объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="38845-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38845-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38845-107">Prerequisites</span></span>
<span data-ttu-id="38845-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38845-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38845-110">Permission type</span></span>|<span data-ttu-id="38845-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38845-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38845-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38845-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38845-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38845-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38845-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38845-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38845-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38845-115">Not supported.</span></span>|
|<span data-ttu-id="38845-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38845-116">Application</span></span>|<span data-ttu-id="38845-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38845-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38845-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38845-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="38845-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38845-119">Request headers</span></span>
|<span data-ttu-id="38845-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38845-120">Header</span></span>|<span data-ttu-id="38845-121">Значение</span><span class="sxs-lookup"><span data-stu-id="38845-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38845-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38845-122">Authorization</span></span>|<span data-ttu-id="38845-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38845-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38845-124">Accept</span><span class="sxs-lookup"><span data-stu-id="38845-124">Accept</span></span>|<span data-ttu-id="38845-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38845-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38845-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38845-126">Request body</span></span>
<span data-ttu-id="38845-127">В тексте запроса добавьте представление объекта [Девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38845-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="38845-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="38845-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="38845-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="38845-129">Property</span></span>|<span data-ttu-id="38845-130">Тип</span><span class="sxs-lookup"><span data-stu-id="38845-130">Type</span></span>|<span data-ttu-id="38845-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38845-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38845-132">id</span><span class="sxs-lookup"><span data-stu-id="38845-132">id</span></span>|<span data-ttu-id="38845-133">String</span><span class="sxs-lookup"><span data-stu-id="38845-133">String</span></span>|<span data-ttu-id="38845-134">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="38845-134">The template ID</span></span>|
|<span data-ttu-id="38845-135">displayName</span><span class="sxs-lookup"><span data-stu-id="38845-135">displayName</span></span>|<span data-ttu-id="38845-136">Строка</span><span class="sxs-lookup"><span data-stu-id="38845-136">String</span></span>|<span data-ttu-id="38845-137">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="38845-137">The template's display name</span></span>|
|<span data-ttu-id="38845-138">description</span><span class="sxs-lookup"><span data-stu-id="38845-138">description</span></span>|<span data-ttu-id="38845-139">String</span><span class="sxs-lookup"><span data-stu-id="38845-139">String</span></span>|<span data-ttu-id="38845-140">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="38845-140">The template's description</span></span>|
|<span data-ttu-id="38845-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="38845-141">versionInfo</span></span>|<span data-ttu-id="38845-142">Строка</span><span class="sxs-lookup"><span data-stu-id="38845-142">String</span></span>|<span data-ttu-id="38845-143">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="38845-143">The template's version information</span></span>|
|<span data-ttu-id="38845-144">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="38845-144">isDeprecated</span></span>|<span data-ttu-id="38845-145">Логический</span><span class="sxs-lookup"><span data-stu-id="38845-145">Boolean</span></span>|<span data-ttu-id="38845-146">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="38845-146">The template is deprecated or not.</span></span> <span data-ttu-id="38845-147">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="38845-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="38845-148">Интенткаунт</span><span class="sxs-lookup"><span data-stu-id="38845-148">intentCount</span></span>|<span data-ttu-id="38845-149">Int32</span><span class="sxs-lookup"><span data-stu-id="38845-149">Int32</span></span>|<span data-ttu-id="38845-150">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="38845-150">Number of Intents created from this template.</span></span>|



## <a name="response"></a><span data-ttu-id="38845-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="38845-151">Response</span></span>
<span data-ttu-id="38845-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38845-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38845-153">Пример</span><span class="sxs-lookup"><span data-stu-id="38845-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="38845-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="38845-154">Request</span></span>
<span data-ttu-id="38845-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38845-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```

### <a name="response"></a><span data-ttu-id="38845-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="38845-156">Response</span></span>
<span data-ttu-id="38845-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38845-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```




