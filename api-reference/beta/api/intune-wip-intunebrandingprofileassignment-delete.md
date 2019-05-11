---
title: Удаление Интунебрандингпрофилеассигнмент
description: Удаляет объект Интунебрандингпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60b631748d2a1b813f8b9b8d63c76b7b3830e748
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898984"
---
# <a name="delete-intunebrandingprofileassignment"></a><span data-ttu-id="aacdb-103">Удаление Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="aacdb-103">Delete intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="aacdb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aacdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aacdb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aacdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aacdb-106">Удаляет объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aacdb-106">Deletes a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aacdb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aacdb-107">Prerequisites</span></span>
<span data-ttu-id="aacdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aacdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aacdb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aacdb-110">Permission type</span></span>|<span data-ttu-id="aacdb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aacdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aacdb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aacdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aacdb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aacdb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aacdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aacdb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aacdb-115">Not supported.</span></span>|
|<span data-ttu-id="aacdb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aacdb-116">Application</span></span>|<span data-ttu-id="aacdb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aacdb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aacdb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aacdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aacdb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aacdb-119">Request headers</span></span>
|<span data-ttu-id="aacdb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aacdb-120">Header</span></span>|<span data-ttu-id="aacdb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aacdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aacdb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aacdb-122">Authorization</span></span>|<span data-ttu-id="aacdb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aacdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aacdb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aacdb-124">Accept</span></span>|<span data-ttu-id="aacdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aacdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aacdb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aacdb-126">Request body</span></span>
<span data-ttu-id="aacdb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aacdb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aacdb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aacdb-128">Response</span></span>
<span data-ttu-id="aacdb-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aacdb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aacdb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aacdb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aacdb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aacdb-131">Request</span></span>
<span data-ttu-id="aacdb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aacdb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="aacdb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aacdb-133">Response</span></span>
<span data-ttu-id="aacdb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aacdb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




