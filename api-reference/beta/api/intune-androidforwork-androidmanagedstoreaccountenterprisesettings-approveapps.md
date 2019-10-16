---
title: действие Аппровеаппс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d5b955a8fb8de5740d854aa3e7d80be7e245f22
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535557"
---
# <a name="approveapps-action"></a><span data-ttu-id="addf5-103">действие Аппровеаппс</span><span class="sxs-lookup"><span data-stu-id="addf5-103">approveApps action</span></span>

> <span data-ttu-id="addf5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="addf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="addf5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="addf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="addf5-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="addf5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="addf5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="addf5-107">Prerequisites</span></span>
<span data-ttu-id="addf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="addf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="addf5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="addf5-110">Permission type</span></span>|<span data-ttu-id="addf5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="addf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="addf5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="addf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="addf5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="addf5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="addf5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="addf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="addf5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="addf5-115">Not supported.</span></span>|
|<span data-ttu-id="addf5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="addf5-116">Application</span></span>|<span data-ttu-id="addf5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="addf5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="addf5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="addf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps
```

## <a name="request-headers"></a><span data-ttu-id="addf5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="addf5-119">Request headers</span></span>
|<span data-ttu-id="addf5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="addf5-120">Header</span></span>|<span data-ttu-id="addf5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="addf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="addf5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="addf5-122">Authorization</span></span>|<span data-ttu-id="addf5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="addf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="addf5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="addf5-124">Accept</span></span>|<span data-ttu-id="addf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="addf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="addf5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="addf5-126">Request body</span></span>
<span data-ttu-id="addf5-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="addf5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="addf5-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="addf5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="addf5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="addf5-129">Property</span></span>|<span data-ttu-id="addf5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="addf5-130">Type</span></span>|<span data-ttu-id="addf5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="addf5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="addf5-132">паккажеидс</span><span class="sxs-lookup"><span data-stu-id="addf5-132">packageIds</span></span>|<span data-ttu-id="addf5-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="addf5-133">String collection</span></span>|<span data-ttu-id="addf5-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="addf5-134">Not yet documented</span></span>|
|<span data-ttu-id="addf5-135">аппровеаллпермиссионс</span><span class="sxs-lookup"><span data-stu-id="addf5-135">approveAllPermissions</span></span>|<span data-ttu-id="addf5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="addf5-136">Boolean</span></span>|<span data-ttu-id="addf5-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="addf5-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="addf5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="addf5-138">Response</span></span>
<span data-ttu-id="addf5-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="addf5-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="addf5-140">Пример</span><span class="sxs-lookup"><span data-stu-id="addf5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="addf5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="addf5-141">Request</span></span>
<span data-ttu-id="addf5-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="addf5-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps

Content-type: application/json
Content-length: 87

{
  "packageIds": [
    "Package Ids value"
  ],
  "approveAllPermissions": true
}
```

### <a name="response"></a><span data-ttu-id="addf5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="addf5-143">Response</span></span>
<span data-ttu-id="addf5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="addf5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






