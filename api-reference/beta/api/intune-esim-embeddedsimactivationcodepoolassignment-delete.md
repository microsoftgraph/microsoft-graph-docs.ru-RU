---
title: Удаление Ембеддедсимактиватионкодепулассигнмент
description: Удаляет объект Ембеддедсимактиватионкодепулассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7da7004845a112acea4e19662dab23e511f6b3f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995309"
---
# <a name="delete-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="b7522-103">Удаление Ембеддедсимактиватионкодепулассигнмент</span><span class="sxs-lookup"><span data-stu-id="b7522-103">Delete embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="b7522-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7522-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7522-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7522-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7522-106">Удаляет объект [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b7522-106">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7522-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b7522-107">Prerequisites</span></span>
<span data-ttu-id="b7522-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7522-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7522-110">Permission type</span></span>|<span data-ttu-id="b7522-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7522-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7522-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7522-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7522-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7522-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7522-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7522-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7522-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7522-115">Not supported.</span></span>|
|<span data-ttu-id="b7522-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7522-116">Application</span></span>|<span data-ttu-id="b7522-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7522-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7522-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7522-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b7522-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7522-119">Request headers</span></span>
|<span data-ttu-id="b7522-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7522-120">Header</span></span>|<span data-ttu-id="b7522-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7522-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7522-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7522-122">Authorization</span></span>|<span data-ttu-id="b7522-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7522-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7522-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7522-124">Accept</span></span>|<span data-ttu-id="b7522-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7522-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7522-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7522-126">Request body</span></span>
<span data-ttu-id="b7522-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7522-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7522-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7522-128">Response</span></span>
<span data-ttu-id="b7522-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b7522-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7522-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b7522-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7522-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7522-131">Request</span></span>
<span data-ttu-id="b7522-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7522-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b7522-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7522-133">Response</span></span>
<span data-ttu-id="b7522-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7522-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





