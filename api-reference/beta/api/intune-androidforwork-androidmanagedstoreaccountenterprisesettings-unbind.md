---
title: Действие unbind
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b62ccf5f72ad6900ff41b39e68058339b61fa8c0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174006"
---
# <a name="unbind-action"></a><span data-ttu-id="d2793-103">Действие unbind</span><span class="sxs-lookup"><span data-stu-id="d2793-103">unbind action</span></span>

> <span data-ttu-id="d2793-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2793-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2793-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2793-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2793-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d2793-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2793-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d2793-107">Prerequisites</span></span>
<span data-ttu-id="d2793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2793-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2793-110">Permission type</span></span>|<span data-ttu-id="d2793-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2793-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2793-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2793-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2793-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2793-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2793-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2793-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2793-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2793-115">Not supported.</span></span>|
|<span data-ttu-id="d2793-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2793-116">Application</span></span>|<span data-ttu-id="d2793-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2793-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2793-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2793-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/unbind
```

## <a name="request-headers"></a><span data-ttu-id="d2793-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2793-119">Request headers</span></span>
|<span data-ttu-id="d2793-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2793-120">Header</span></span>|<span data-ttu-id="d2793-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2793-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2793-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2793-122">Authorization</span></span>|<span data-ttu-id="d2793-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2793-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2793-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d2793-124">Accept</span></span>|<span data-ttu-id="d2793-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2793-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2793-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2793-126">Request body</span></span>
<span data-ttu-id="d2793-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2793-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2793-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2793-128">Response</span></span>
<span data-ttu-id="d2793-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2793-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2793-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d2793-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2793-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2793-131">Request</span></span>
<span data-ttu-id="d2793-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2793-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/unbind
```

### <a name="response"></a><span data-ttu-id="d2793-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2793-133">Response</span></span>
<span data-ttu-id="d2793-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2793-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




