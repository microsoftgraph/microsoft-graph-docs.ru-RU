---
title: удалить действие
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b811d6803a14ad57b316120d44fe085e0b3d239b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224741"
---
# <a name="remove-action"></a><span data-ttu-id="12675-103">удалить действие</span><span class="sxs-lookup"><span data-stu-id="12675-103">remove action</span></span>

<span data-ttu-id="12675-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12675-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12675-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12675-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12675-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12675-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12675-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="12675-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12675-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12675-108">Prerequisites</span></span>
<span data-ttu-id="12675-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12675-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12675-111">Permission type</span></span>|<span data-ttu-id="12675-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12675-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12675-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12675-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12675-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12675-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12675-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12675-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12675-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12675-116">Not supported.</span></span>|
|<span data-ttu-id="12675-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="12675-117">Application</span></span>|<span data-ttu-id="12675-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12675-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12675-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12675-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/remove
```

## <a name="request-headers"></a><span data-ttu-id="12675-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12675-120">Request headers</span></span>
|<span data-ttu-id="12675-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12675-121">Header</span></span>|<span data-ttu-id="12675-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12675-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12675-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12675-123">Authorization</span></span>|<span data-ttu-id="12675-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12675-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12675-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12675-125">Accept</span></span>|<span data-ttu-id="12675-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12675-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12675-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12675-127">Request body</span></span>
<span data-ttu-id="12675-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12675-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12675-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="12675-129">Response</span></span>
<span data-ttu-id="12675-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="12675-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="12675-131">Пример</span><span class="sxs-lookup"><span data-stu-id="12675-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="12675-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="12675-132">Request</span></span>
<span data-ttu-id="12675-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12675-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles/{groupPolicyUploadedDefinitionFileId}/remove
```

### <a name="response"></a><span data-ttu-id="12675-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="12675-134">Response</span></span>
<span data-ttu-id="12675-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12675-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




