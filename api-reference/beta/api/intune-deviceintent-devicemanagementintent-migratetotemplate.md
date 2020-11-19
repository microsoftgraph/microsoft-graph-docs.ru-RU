---
title: действие Мигратетотемплате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c8f64abfd7e214f3dff486c2b01dd514096f316
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229760"
---
# <a name="migratetotemplate-action"></a><span data-ttu-id="1ceb4-103">действие Мигратетотемплате</span><span class="sxs-lookup"><span data-stu-id="1ceb4-103">migrateToTemplate action</span></span>

<span data-ttu-id="1ceb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ceb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ceb4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ceb4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ceb4-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ceb4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1ceb4-108">Prerequisites</span></span>
<span data-ttu-id="1ceb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ceb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ceb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ceb4-111">Permission type</span></span>|<span data-ttu-id="1ceb4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ceb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ceb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ceb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ceb4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ceb4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ceb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ceb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ceb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-116">Not supported.</span></span>|
|<span data-ttu-id="1ceb4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1ceb4-117">Application</span></span>|<span data-ttu-id="1ceb4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ceb4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ceb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ceb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate
```

## <a name="request-headers"></a><span data-ttu-id="1ceb4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1ceb4-120">Request headers</span></span>
|<span data-ttu-id="1ceb4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ceb4-121">Header</span></span>|<span data-ttu-id="1ceb4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ceb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ceb4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ceb4-123">Authorization</span></span>|<span data-ttu-id="1ceb4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ceb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ceb4-125">Accept</span></span>|<span data-ttu-id="1ceb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ceb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ceb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ceb4-127">Request body</span></span>
<span data-ttu-id="1ceb4-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1ceb4-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1ceb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ceb4-130">Property</span></span>|<span data-ttu-id="1ceb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ceb4-131">Type</span></span>|<span data-ttu-id="1ceb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ceb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ceb4-133">невтемплатеид</span><span class="sxs-lookup"><span data-stu-id="1ceb4-133">newTemplateId</span></span>|<span data-ttu-id="1ceb4-134">String</span><span class="sxs-lookup"><span data-stu-id="1ceb4-134">String</span></span>|<span data-ttu-id="1ceb4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-135">Not yet documented</span></span>|
|<span data-ttu-id="1ceb4-136">пресервекустомвалуес</span><span class="sxs-lookup"><span data-stu-id="1ceb4-136">preserveCustomValues</span></span>|<span data-ttu-id="1ceb4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ceb4-137">Boolean</span></span>|<span data-ttu-id="1ceb4-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1ceb4-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1ceb4-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ceb4-139">Response</span></span>
<span data-ttu-id="1ceb4-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1ceb4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1ceb4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ceb4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ceb4-142">Request</span></span>
<span data-ttu-id="1ceb4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/migrateToTemplate

Content-type: application/json
Content-length: 81

{
  "newTemplateId": "New Template Id value",
  "preserveCustomValues": true
}
```

### <a name="response"></a><span data-ttu-id="1ceb4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ceb4-144">Response</span></span>
<span data-ttu-id="1ceb4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ceb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




