---
title: Обновление Секуритибаселинетемплате
description: Обновление свойств объекта Секуритибаселинетемплате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d407646c4369352d8ce8f1760c5a64f4d99dbc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522771"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="787dd-103">Обновление Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="787dd-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="787dd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="787dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="787dd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="787dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="787dd-106">Обновление свойств объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="787dd-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="787dd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="787dd-107">Prerequisites</span></span>
<span data-ttu-id="787dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="787dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="787dd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="787dd-110">Permission type</span></span>|<span data-ttu-id="787dd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="787dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="787dd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="787dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="787dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="787dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="787dd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="787dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="787dd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="787dd-115">Not supported.</span></span>|
|<span data-ttu-id="787dd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="787dd-116">Application</span></span>|<span data-ttu-id="787dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="787dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="787dd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="787dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="787dd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="787dd-119">Request headers</span></span>
|<span data-ttu-id="787dd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="787dd-120">Header</span></span>|<span data-ttu-id="787dd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="787dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="787dd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="787dd-122">Authorization</span></span>|<span data-ttu-id="787dd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="787dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="787dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="787dd-124">Accept</span></span>|<span data-ttu-id="787dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="787dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="787dd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="787dd-126">Request body</span></span>
<span data-ttu-id="787dd-127">В тексте запроса добавьте представление объекта [Секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="787dd-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="787dd-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="787dd-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="787dd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="787dd-129">Property</span></span>|<span data-ttu-id="787dd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="787dd-130">Type</span></span>|<span data-ttu-id="787dd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="787dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="787dd-132">id</span><span class="sxs-lookup"><span data-stu-id="787dd-132">id</span></span>|<span data-ttu-id="787dd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="787dd-133">String</span></span>|<span data-ttu-id="787dd-134">Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="787dd-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="787dd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="787dd-135">displayName</span></span>|<span data-ttu-id="787dd-136">String</span><span class="sxs-lookup"><span data-stu-id="787dd-136">String</span></span>|<span data-ttu-id="787dd-137">Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="787dd-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="787dd-138">description</span><span class="sxs-lookup"><span data-stu-id="787dd-138">description</span></span>|<span data-ttu-id="787dd-139">String</span><span class="sxs-lookup"><span data-stu-id="787dd-139">String</span></span>|<span data-ttu-id="787dd-140">Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="787dd-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="787dd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="787dd-141">Response</span></span>
<span data-ttu-id="787dd-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="787dd-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="787dd-143">Пример</span><span class="sxs-lookup"><span data-stu-id="787dd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="787dd-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="787dd-144">Request</span></span>
<span data-ttu-id="787dd-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="787dd-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="787dd-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="787dd-146">Response</span></span>
<span data-ttu-id="787dd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="787dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```







