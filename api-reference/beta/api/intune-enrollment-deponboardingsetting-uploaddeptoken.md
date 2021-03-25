---
title: Действие uploadDepToken
description: Загрузка нового маркера программы регистрации устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d302676b16f29e7f004081b78d77c4fc2a610e48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153918"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="d4aa7-103">Действие uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="d4aa7-103">uploadDepToken action</span></span>

<span data-ttu-id="d4aa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4aa7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4aa7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4aa7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4aa7-107">Загрузка нового маркера программы регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d4aa7-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4aa7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4aa7-108">Prerequisites</span></span>
<span data-ttu-id="d4aa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4aa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4aa7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4aa7-111">Permission type</span></span>|<span data-ttu-id="d4aa7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4aa7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4aa7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4aa7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4aa7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4aa7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4aa7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4aa7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4aa7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-116">Not supported.</span></span>|
|<span data-ttu-id="d4aa7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4aa7-117">Application</span></span>|<span data-ttu-id="d4aa7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4aa7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4aa7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4aa7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="d4aa7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4aa7-120">Request headers</span></span>
|<span data-ttu-id="d4aa7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4aa7-121">Header</span></span>|<span data-ttu-id="d4aa7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4aa7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4aa7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4aa7-123">Authorization</span></span>|<span data-ttu-id="d4aa7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4aa7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4aa7-125">Accept</span></span>|<span data-ttu-id="d4aa7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4aa7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4aa7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4aa7-127">Request body</span></span>
<span data-ttu-id="d4aa7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d4aa7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d4aa7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4aa7-130">Property</span></span>|<span data-ttu-id="d4aa7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4aa7-131">Type</span></span>|<span data-ttu-id="d4aa7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4aa7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4aa7-133">appleId</span><span class="sxs-lookup"><span data-stu-id="d4aa7-133">appleId</span></span>|<span data-ttu-id="d4aa7-134">String</span><span class="sxs-lookup"><span data-stu-id="d4aa7-134">String</span></span>|<span data-ttu-id="d4aa7-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-135">Not yet documented</span></span>|
|<span data-ttu-id="d4aa7-136">depToken</span><span class="sxs-lookup"><span data-stu-id="d4aa7-136">depToken</span></span>|<span data-ttu-id="d4aa7-137">String</span><span class="sxs-lookup"><span data-stu-id="d4aa7-137">String</span></span>|<span data-ttu-id="d4aa7-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d4aa7-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4aa7-139">Response</span></span>
<span data-ttu-id="d4aa7-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d4aa7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d4aa7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4aa7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4aa7-142">Request</span></span>
<span data-ttu-id="d4aa7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="d4aa7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4aa7-144">Response</span></span>
<span data-ttu-id="d4aa7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4aa7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




