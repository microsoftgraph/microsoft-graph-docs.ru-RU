---
title: Действие uploadDepToken
description: Отправка нового маркера программы регистрации устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ea0a8ce6984ba5598cc42a04a9d3799aa50a10e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908639"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="0a248-103">Действие uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="0a248-103">uploadDepToken action</span></span>

> <span data-ttu-id="0a248-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a248-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a248-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a248-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a248-106">Отправка нового маркера программы регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="0a248-106">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a248-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a248-107">Prerequisites</span></span>
<span data-ttu-id="0a248-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a248-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a248-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a248-110">Permission type</span></span>|<span data-ttu-id="0a248-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a248-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a248-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a248-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a248-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a248-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a248-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a248-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a248-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a248-115">Not supported.</span></span>|
|<span data-ttu-id="0a248-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a248-116">Application</span></span>|<span data-ttu-id="0a248-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a248-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a248-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a248-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="0a248-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a248-119">Request headers</span></span>
|<span data-ttu-id="0a248-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a248-120">Header</span></span>|<span data-ttu-id="0a248-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0a248-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a248-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a248-122">Authorization</span></span>|<span data-ttu-id="0a248-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a248-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a248-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0a248-124">Accept</span></span>|<span data-ttu-id="0a248-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a248-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a248-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a248-126">Request body</span></span>
<span data-ttu-id="0a248-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a248-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0a248-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0a248-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0a248-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a248-129">Property</span></span>|<span data-ttu-id="0a248-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0a248-130">Type</span></span>|<span data-ttu-id="0a248-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0a248-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a248-132">appleId</span><span class="sxs-lookup"><span data-stu-id="0a248-132">appleId</span></span>|<span data-ttu-id="0a248-133">String</span><span class="sxs-lookup"><span data-stu-id="0a248-133">String</span></span>|<span data-ttu-id="0a248-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0a248-134">Not yet documented</span></span>|
|<span data-ttu-id="0a248-135">Дептокен</span><span class="sxs-lookup"><span data-stu-id="0a248-135">depToken</span></span>|<span data-ttu-id="0a248-136">String</span><span class="sxs-lookup"><span data-stu-id="0a248-136">String</span></span>|<span data-ttu-id="0a248-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0a248-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a248-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a248-138">Response</span></span>
<span data-ttu-id="0a248-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a248-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a248-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0a248-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a248-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a248-141">Request</span></span>
<span data-ttu-id="0a248-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a248-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="0a248-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a248-143">Response</span></span>
<span data-ttu-id="0a248-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a248-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




