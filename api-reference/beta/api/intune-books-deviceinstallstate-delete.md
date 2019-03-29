---
title: Delete deviceInstallState
description: Удаляет объект deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 675d62032a9e5bd4543a098445fbf62bf0853f70
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965405"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="46820-103">Delete deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="46820-103">Delete deviceInstallState</span></span>

> <span data-ttu-id="46820-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46820-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46820-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46820-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46820-106">Удаляет объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="46820-106">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46820-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="46820-107">Prerequisites</span></span>
<span data-ttu-id="46820-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46820-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46820-110">Permission type</span></span>|<span data-ttu-id="46820-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46820-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46820-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46820-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46820-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46820-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46820-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46820-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46820-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46820-115">Not supported.</span></span>|
|<span data-ttu-id="46820-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46820-116">Application</span></span>|<span data-ttu-id="46820-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46820-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46820-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46820-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="46820-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46820-119">Request headers</span></span>
|<span data-ttu-id="46820-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46820-120">Header</span></span>|<span data-ttu-id="46820-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46820-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46820-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46820-122">Authorization</span></span>|<span data-ttu-id="46820-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46820-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46820-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46820-124">Accept</span></span>|<span data-ttu-id="46820-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46820-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46820-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46820-126">Request body</span></span>
<span data-ttu-id="46820-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46820-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46820-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="46820-128">Response</span></span>
<span data-ttu-id="46820-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46820-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46820-130">Пример</span><span class="sxs-lookup"><span data-stu-id="46820-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46820-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="46820-131">Request</span></span>
<span data-ttu-id="46820-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46820-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="46820-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="46820-133">Response</span></span>
<span data-ttu-id="46820-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46820-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




