---
title: Действие unbind
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4931363ff3fe47480a2b2dcc15e313bf62d74a88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952662"
---
# <a name="unbind-action"></a><span data-ttu-id="6b597-103">Действие unbind</span><span class="sxs-lookup"><span data-stu-id="6b597-103">unbind action</span></span>

> <span data-ttu-id="6b597-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b597-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b597-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b597-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b597-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6b597-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b597-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6b597-107">Prerequisites</span></span>
<span data-ttu-id="6b597-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b597-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b597-110">Permission type</span></span>|<span data-ttu-id="6b597-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b597-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b597-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b597-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b597-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b597-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b597-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b597-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b597-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b597-115">Not supported.</span></span>|
|<span data-ttu-id="6b597-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b597-116">Application</span></span>|<span data-ttu-id="6b597-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b597-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b597-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b597-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/unbind
```

## <a name="request-headers"></a><span data-ttu-id="6b597-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b597-119">Request headers</span></span>
|<span data-ttu-id="6b597-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b597-120">Header</span></span>|<span data-ttu-id="6b597-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b597-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b597-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b597-122">Authorization</span></span>|<span data-ttu-id="6b597-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b597-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b597-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6b597-124">Accept</span></span>|<span data-ttu-id="6b597-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b597-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b597-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6b597-126">Request body</span></span>
<span data-ttu-id="6b597-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b597-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b597-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b597-128">Response</span></span>
<span data-ttu-id="6b597-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6b597-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6b597-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6b597-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b597-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b597-131">Request</span></span>
<span data-ttu-id="6b597-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b597-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/unbind
```

### <a name="response"></a><span data-ttu-id="6b597-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b597-133">Response</span></span>
<span data-ttu-id="6b597-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b597-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





