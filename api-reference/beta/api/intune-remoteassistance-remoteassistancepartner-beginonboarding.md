---
title: Действие beginOnboarding
description: Запрос на запуск входящей миграции.  Должен быть связан с соответствующими сведениями учетной записи TeamViewer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36fa3b2d27bbcad94ad2427c5a248a3ae5360fc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527240"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="e2f81-104">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="e2f81-104">beginOnboarding action</span></span>

> <span data-ttu-id="e2f81-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2f81-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2f81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2f81-107">Запрос на запуск входящей миграции.</span><span class="sxs-lookup"><span data-stu-id="e2f81-107">A request to start onboarding.</span></span>  <span data-ttu-id="e2f81-108">Должен быть связан с соответствующими сведениями учетной записи TeamViewer</span><span class="sxs-lookup"><span data-stu-id="e2f81-108">Must be coupled with the appropriate TeamViewer account information</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2f81-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2f81-109">Prerequisites</span></span>
<span data-ttu-id="e2f81-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2f81-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2f81-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f81-112">Permission type</span></span>|<span data-ttu-id="e2f81-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2f81-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2f81-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2f81-114">Delegated (work or school account)</span></span>|<span data-ttu-id="e2f81-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f81-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e2f81-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2f81-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2f81-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f81-117">Not supported.</span></span>|
|<span data-ttu-id="e2f81-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2f81-118">Application</span></span>|<span data-ttu-id="e2f81-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f81-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2f81-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2f81-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="e2f81-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2f81-121">Request headers</span></span>
|<span data-ttu-id="e2f81-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2f81-122">Header</span></span>|<span data-ttu-id="e2f81-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e2f81-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2f81-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2f81-124">Authorization</span></span>|<span data-ttu-id="e2f81-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2f81-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2f81-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e2f81-126">Accept</span></span>|<span data-ttu-id="e2f81-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2f81-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2f81-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2f81-128">Request body</span></span>
<span data-ttu-id="e2f81-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2f81-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2f81-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2f81-130">Response</span></span>
<span data-ttu-id="e2f81-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e2f81-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e2f81-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e2f81-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2f81-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2f81-133">Request</span></span>
<span data-ttu-id="e2f81-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2f81-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="e2f81-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f81-135">Response</span></span>
<span data-ttu-id="e2f81-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2f81-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





