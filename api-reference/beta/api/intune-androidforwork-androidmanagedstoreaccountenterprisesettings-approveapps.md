---
title: действие Аппровеаппс
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7cbe77613d13e0515f0f473ea801456b35dc143
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762519"
---
# <a name="approveapps-action"></a><span data-ttu-id="01f08-103">действие Аппровеаппс</span><span class="sxs-lookup"><span data-stu-id="01f08-103">approveApps action</span></span>

> <span data-ttu-id="01f08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01f08-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01f08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01f08-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="01f08-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01f08-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01f08-107">Prerequisites</span></span>
<span data-ttu-id="01f08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01f08-110">Permission type</span></span>|<span data-ttu-id="01f08-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01f08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01f08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01f08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01f08-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f08-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01f08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01f08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01f08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f08-115">Not supported.</span></span>|
|<span data-ttu-id="01f08-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="01f08-116">Application</span></span>|<span data-ttu-id="01f08-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f08-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01f08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01f08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/approveApps
```

## <a name="request-headers"></a><span data-ttu-id="01f08-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01f08-119">Request headers</span></span>
|<span data-ttu-id="01f08-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01f08-120">Header</span></span>|<span data-ttu-id="01f08-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01f08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01f08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f08-122">Authorization</span></span>|<span data-ttu-id="01f08-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01f08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01f08-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01f08-124">Accept</span></span>|<span data-ttu-id="01f08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01f08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f08-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01f08-126">Request body</span></span>
<span data-ttu-id="01f08-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01f08-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="01f08-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="01f08-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="01f08-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01f08-129">Property</span></span>|<span data-ttu-id="01f08-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01f08-130">Type</span></span>|<span data-ttu-id="01f08-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01f08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01f08-132">паккажеидс</span><span class="sxs-lookup"><span data-stu-id="01f08-132">packageIds</span></span>|<span data-ttu-id="01f08-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="01f08-133">String collection</span></span>|<span data-ttu-id="01f08-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="01f08-134">Not yet documented</span></span>|
|<span data-ttu-id="01f08-135">аппровеаллпермиссионс</span><span class="sxs-lookup"><span data-stu-id="01f08-135">approveAllPermissions</span></span>|<span data-ttu-id="01f08-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="01f08-136">Boolean</span></span>|<span data-ttu-id="01f08-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="01f08-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="01f08-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="01f08-138">Response</span></span>
<span data-ttu-id="01f08-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="01f08-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="01f08-140">Пример</span><span class="sxs-lookup"><span data-stu-id="01f08-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="01f08-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="01f08-141">Request</span></span>
<span data-ttu-id="01f08-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01f08-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01f08-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f08-143">Response</span></span>
<span data-ttu-id="01f08-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01f08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




