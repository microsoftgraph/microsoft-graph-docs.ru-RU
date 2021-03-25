---
title: включить действие
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6cc9664a75e3afc73008c6cd4d88013286343ce
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159483"
---
# <a name="enable-action"></a><span data-ttu-id="82d82-103">включить действие</span><span class="sxs-lookup"><span data-stu-id="82d82-103">enable action</span></span>

<span data-ttu-id="82d82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82d82-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82d82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82d82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d82-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="82d82-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82d82-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82d82-108">Prerequisites</span></span>
<span data-ttu-id="82d82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82d82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82d82-111">Permission type</span></span>|<span data-ttu-id="82d82-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82d82-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82d82-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82d82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82d82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82d82-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82d82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82d82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d82-116">Not supported.</span></span>|
|<span data-ttu-id="82d82-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="82d82-117">Application</span></span>|<span data-ttu-id="82d82-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d82-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82d82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82d82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters/enable
```

## <a name="request-headers"></a><span data-ttu-id="82d82-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82d82-120">Request headers</span></span>
|<span data-ttu-id="82d82-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82d82-121">Header</span></span>|<span data-ttu-id="82d82-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82d82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82d82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d82-123">Authorization</span></span>|<span data-ttu-id="82d82-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82d82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82d82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82d82-125">Accept</span></span>|<span data-ttu-id="82d82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82d82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82d82-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82d82-127">Request body</span></span>
<span data-ttu-id="82d82-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82d82-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82d82-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="82d82-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82d82-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="82d82-130">Property</span></span>|<span data-ttu-id="82d82-131">Тип</span><span class="sxs-lookup"><span data-stu-id="82d82-131">Type</span></span>|<span data-ttu-id="82d82-132">Описание</span><span class="sxs-lookup"><span data-stu-id="82d82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d82-133">включить</span><span class="sxs-lookup"><span data-stu-id="82d82-133">enable</span></span>|<span data-ttu-id="82d82-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="82d82-134">Boolean</span></span>|<span data-ttu-id="82d82-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="82d82-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82d82-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="82d82-136">Response</span></span>
<span data-ttu-id="82d82-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="82d82-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82d82-138">Пример</span><span class="sxs-lookup"><span data-stu-id="82d82-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="82d82-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="82d82-139">Request</span></span>
<span data-ttu-id="82d82-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82d82-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/enable

Content-type: application/json
Content-length: 22

{
  "enable": true
}
```

### <a name="response"></a><span data-ttu-id="82d82-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d82-141">Response</span></span>
<span data-ttu-id="82d82-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82d82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




