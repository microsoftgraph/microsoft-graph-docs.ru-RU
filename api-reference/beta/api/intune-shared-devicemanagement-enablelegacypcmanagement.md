---
title: Действие enableLegacyPcManagement
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aefec17df5d16ab2df908a0899535592ed4e7d7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993636"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="6c841-103">Действие enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="6c841-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="6c841-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6c841-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c841-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c841-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c841-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c841-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c841-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6c841-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c841-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6c841-108">Prerequisites</span></span>
<span data-ttu-id="6c841-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c841-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c841-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c841-111">Permission type</span></span>|<span data-ttu-id="6c841-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c841-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c841-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c841-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6c841-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="6c841-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6c841-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c841-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c841-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c841-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c841-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c841-117">Not supported.</span></span>|
|<span data-ttu-id="6c841-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c841-118">Application</span></span>|<span data-ttu-id="6c841-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c841-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c841-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c841-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="6c841-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c841-121">Request headers</span></span>
|<span data-ttu-id="6c841-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c841-122">Header</span></span>|<span data-ttu-id="6c841-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6c841-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c841-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c841-124">Authorization</span></span>|<span data-ttu-id="6c841-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c841-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c841-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6c841-126">Accept</span></span>|<span data-ttu-id="6c841-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c841-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c841-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c841-128">Request body</span></span>
<span data-ttu-id="6c841-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c841-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c841-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c841-130">Response</span></span>
<span data-ttu-id="6c841-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c841-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c841-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6c841-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c841-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c841-133">Request</span></span>
<span data-ttu-id="6c841-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c841-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="6c841-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c841-135">Response</span></span>
<span data-ttu-id="6c841-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c841-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





