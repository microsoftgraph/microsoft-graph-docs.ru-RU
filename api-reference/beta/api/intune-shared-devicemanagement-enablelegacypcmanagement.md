---
title: Действие enableLegacyPcManagement
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ea5e5f8639dd59d91ec30102fd5a7c9a017622a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527128"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="84f49-103">Действие enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="84f49-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="84f49-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84f49-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84f49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84f49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84f49-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84f49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84f49-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84f49-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84f49-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="84f49-108">Prerequisites</span></span>
<span data-ttu-id="84f49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84f49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84f49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84f49-111">Permission type</span></span>|<span data-ttu-id="84f49-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84f49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84f49-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84f49-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="84f49-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="84f49-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="84f49-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84f49-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84f49-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84f49-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84f49-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84f49-117">Not supported.</span></span>|
|<span data-ttu-id="84f49-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84f49-118">Application</span></span>|<span data-ttu-id="84f49-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84f49-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84f49-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84f49-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="84f49-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84f49-121">Request headers</span></span>
|<span data-ttu-id="84f49-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84f49-122">Header</span></span>|<span data-ttu-id="84f49-123">Значение</span><span class="sxs-lookup"><span data-stu-id="84f49-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84f49-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84f49-124">Authorization</span></span>|<span data-ttu-id="84f49-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84f49-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84f49-126">Accept</span><span class="sxs-lookup"><span data-stu-id="84f49-126">Accept</span></span>|<span data-ttu-id="84f49-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84f49-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84f49-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84f49-128">Request body</span></span>
<span data-ttu-id="84f49-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84f49-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84f49-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="84f49-130">Response</span></span>
<span data-ttu-id="84f49-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="84f49-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84f49-132">Пример</span><span class="sxs-lookup"><span data-stu-id="84f49-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="84f49-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="84f49-133">Request</span></span>
<span data-ttu-id="84f49-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84f49-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="84f49-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="84f49-135">Response</span></span>
<span data-ttu-id="84f49-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84f49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





