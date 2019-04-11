---
title: Действие beginOnboarding
description: Запрос на запуск входящей миграции.  Должен быть связан с соответствующими сведениями учетной записи TeamViewer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36fa3b2d27bbcad94ad2427c5a248a3ae5360fc8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789873"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="496d7-104">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="496d7-104">beginOnboarding action</span></span>

> <span data-ttu-id="496d7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="496d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="496d7-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="496d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="496d7-107">Запрос на запуск входящей миграции.</span><span class="sxs-lookup"><span data-stu-id="496d7-107">A request to start onboarding.</span></span>  <span data-ttu-id="496d7-108">Должен быть связан с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="496d7-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="496d7-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="496d7-109">Prerequisites</span></span>
<span data-ttu-id="496d7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="496d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="496d7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="496d7-112">Permission type</span></span>|<span data-ttu-id="496d7-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="496d7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="496d7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="496d7-114">Delegated (work or school account)</span></span>|<span data-ttu-id="496d7-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496d7-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="496d7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="496d7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="496d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="496d7-117">Not supported.</span></span>|
|<span data-ttu-id="496d7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="496d7-118">Application</span></span>|<span data-ttu-id="496d7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="496d7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="496d7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="496d7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="496d7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="496d7-121">Request headers</span></span>
|<span data-ttu-id="496d7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="496d7-122">Header</span></span>|<span data-ttu-id="496d7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="496d7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="496d7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="496d7-124">Authorization</span></span>|<span data-ttu-id="496d7-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="496d7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="496d7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="496d7-126">Accept</span></span>|<span data-ttu-id="496d7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="496d7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="496d7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="496d7-128">Request body</span></span>
<span data-ttu-id="496d7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="496d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="496d7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="496d7-130">Response</span></span>
<span data-ttu-id="496d7-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="496d7-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="496d7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="496d7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="496d7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="496d7-133">Request</span></span>
<span data-ttu-id="496d7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="496d7-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="496d7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="496d7-135">Response</span></span>
<span data-ttu-id="496d7-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="496d7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





