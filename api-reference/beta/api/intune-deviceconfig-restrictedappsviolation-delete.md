---
title: Удаление Рестриктедаппсвиолатион
description: Удаляет объект Рестриктедаппсвиолатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5bc23798046255d9d7c8f9b61ed921abae25bbb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922741"
---
# <a name="delete-restrictedappsviolation"></a><span data-ttu-id="45516-103">Удаление Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="45516-103">Delete restrictedAppsViolation</span></span>

> <span data-ttu-id="45516-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45516-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45516-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45516-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45516-106">Удаляет объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="45516-106">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45516-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45516-107">Prerequisites</span></span>
<span data-ttu-id="45516-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45516-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45516-110">Permission type</span></span>|<span data-ttu-id="45516-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45516-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45516-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45516-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45516-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45516-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45516-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45516-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45516-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45516-115">Not supported.</span></span>|
|<span data-ttu-id="45516-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45516-116">Application</span></span>|<span data-ttu-id="45516-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45516-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45516-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45516-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="45516-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45516-119">Request headers</span></span>
|<span data-ttu-id="45516-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45516-120">Header</span></span>|<span data-ttu-id="45516-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45516-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45516-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45516-122">Authorization</span></span>|<span data-ttu-id="45516-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45516-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45516-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45516-124">Accept</span></span>|<span data-ttu-id="45516-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45516-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45516-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45516-126">Request body</span></span>
<span data-ttu-id="45516-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45516-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45516-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="45516-128">Response</span></span>
<span data-ttu-id="45516-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45516-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45516-130">Пример</span><span class="sxs-lookup"><span data-stu-id="45516-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="45516-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45516-131">Request</span></span>
<span data-ttu-id="45516-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45516-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="45516-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="45516-133">Response</span></span>
<span data-ttu-id="45516-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45516-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




