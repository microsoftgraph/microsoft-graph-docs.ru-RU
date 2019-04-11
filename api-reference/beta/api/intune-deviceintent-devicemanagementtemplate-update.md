---
title: Обновление Девицеманажементтемплате
description: Обновление свойств объекта Девицеманажементтемплате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d974ec691b99ecc9f3067f20ab4d2310cbe27d23
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799925"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="e5fe9-103">Обновление Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="e5fe9-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="e5fe9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5fe9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5fe9-106">Обновление свойств объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="e5fe9-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5fe9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5fe9-107">Prerequisites</span></span>
<span data-ttu-id="e5fe9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5fe9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5fe9-110">Permission type</span></span>|<span data-ttu-id="e5fe9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5fe9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5fe9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5fe9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5fe9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5fe9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5fe9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5fe9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5fe9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-115">Not supported.</span></span>|
|<span data-ttu-id="e5fe9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5fe9-116">Application</span></span>|<span data-ttu-id="e5fe9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5fe9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5fe9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="e5fe9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5fe9-119">Request headers</span></span>
|<span data-ttu-id="e5fe9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5fe9-120">Header</span></span>|<span data-ttu-id="e5fe9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5fe9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5fe9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5fe9-122">Authorization</span></span>|<span data-ttu-id="e5fe9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5fe9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5fe9-124">Accept</span></span>|<span data-ttu-id="e5fe9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5fe9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5fe9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5fe9-126">Request body</span></span>
<span data-ttu-id="e5fe9-127">В тексте запроса добавьте представление объекта [Девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="e5fe9-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e5fe9-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="e5fe9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5fe9-129">Property</span></span>|<span data-ttu-id="e5fe9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5fe9-130">Type</span></span>|<span data-ttu-id="e5fe9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5fe9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5fe9-132">id</span><span class="sxs-lookup"><span data-stu-id="e5fe9-132">id</span></span>|<span data-ttu-id="e5fe9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e5fe9-133">String</span></span>|<span data-ttu-id="e5fe9-134">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="e5fe9-134">The template ID</span></span>|
|<span data-ttu-id="e5fe9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e5fe9-135">displayName</span></span>|<span data-ttu-id="e5fe9-136">String</span><span class="sxs-lookup"><span data-stu-id="e5fe9-136">String</span></span>|<span data-ttu-id="e5fe9-137">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="e5fe9-137">The template's display name</span></span>|
|<span data-ttu-id="e5fe9-138">description</span><span class="sxs-lookup"><span data-stu-id="e5fe9-138">description</span></span>|<span data-ttu-id="e5fe9-139">String</span><span class="sxs-lookup"><span data-stu-id="e5fe9-139">String</span></span>|<span data-ttu-id="e5fe9-140">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="e5fe9-140">The template's description</span></span>|



## <a name="response"></a><span data-ttu-id="e5fe9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5fe9-141">Response</span></span>
<span data-ttu-id="e5fe9-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5fe9-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e5fe9-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5fe9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5fe9-144">Request</span></span>
<span data-ttu-id="e5fe9-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="e5fe9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5fe9-146">Response</span></span>
<span data-ttu-id="e5fe9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5fe9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





